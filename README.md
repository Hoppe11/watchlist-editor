# Watchlist Editor V3.3 – repariert

Verbesserungen:
- Passwortänderung wird nach dem Schreiben sofort wieder aus localStorage gelesen.
- Neues Passwort wird testweise entschlüsselt; erst dann meldet die App Erfolg.
- Start prüft, ob localStorage und WebCrypto verfügbar sind.
- Beschädigte Zugangsdaten führen nicht mehr zu einem leeren Bildschirm.
- Entsperren unterscheidet zwischen falschem Passwort und GitHub-/Watchlist-Fehler.
- Sichtbare Startfehler statt stiller JavaScript-Abbrüche.
- Cache-Buster im Manifest (`?v=3.3`).

Sicherheit:
Das Passwort selbst wird nicht gespeichert. Es dient nur zur Verschlüsselung des
GitHub-Tokens im lokalen iPhone-Speicher.
