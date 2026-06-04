# ⚡ VoltPilot

Dashboard GPS + BMS per e-bike con batteria JBD/Xiaoxiang.

## Funzioni Free
- Velocità in tempo reale (GPS)
- Distanza e ODO
- % batteria e autonomia stimata
- Storico ultimi 5 viaggi
- Modalità sole (alta leggibilità)
- Shortcut Telefono, Maps, Spotify

## Funzioni Pro (€2.99)
- Celle batteria individuali in tempo reale
- Meteo in tempo reale
- Storico viaggi illimitato

## Compatibilità BMS
- JBD / Xiaoxiang (SP14S004 e simili)
- Protocollo UART via BLE (UUID ff00/ff01/ff02)

## Come scaricare l'APK
1. Vai su [Releases](../../releases)
2. Scarica l'ultimo `app-debug.apk`
3. Su Android: Impostazioni → Sicurezza → Sorgenti sconosciute
4. Installa il file APK

## Build locale
```bash
npm install
npx cap add android
npx cap sync
cd android && ./gradlew assembleDebug
```

## Tecnologie
- HTML/CSS/JS puro
- Capacitor 5 (wrapper Android)
- Web Bluetooth API (BMS)
- Geolocation API (GPS)
- Open-Meteo API (meteo, no key)
- GitHub Actions (CI/CD)
