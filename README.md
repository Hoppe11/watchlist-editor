# Watchlist Editor V3.5 – PAT-Diagnose

Neu:
- entfernt Leerzeichen/Zeilenumbrüche aus eingefügten Tokens
- prüft zuerst GitHub `/user`
- unterscheidet:
  - PAT ungültig -> 401
  - PAT gültig, Repo/Datei nicht erreichbar -> 404
  - PAT gültig, Rechte unzureichend -> 403
- erst danach wird die Watchlist geladen
- GitHub API-Version auf 2026-03-10 aktualisiert

Der Token wird niemals im Klartext in einer Fehlermeldung ausgegeben.
