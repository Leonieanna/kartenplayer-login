# Kartenspieler – Spotify-Login

Weiterleitungsseite für die Spotify-Anmeldung des Kartenspielers (ESP32).

Spotify verlangt für den Login eine HTTPS-Adresse, die der Player im Heimnetz nicht hat.
Diese Seite nimmt den Login-Code von Spotify entgegen und leitet ihn an den Player im
eigenen WLAN weiter (`http://<player>/callback`). Sie speichert nichts und enthält keine
Geheimnisse – der Login nutzt PKCE, ein Client Secret wird nicht verwendet.

Adresse: <https://leonieanna.github.io/kartenplayer-login/>
