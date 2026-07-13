### Git: Änderungen auf GitHub und lokal zusammenführen

Wenn zwischenzeitlich Änderungen direkt auf GitHub vorgenommen wurden (z. B. eine License hinzugefügt oder geändert) und du gleichzeitig lokale Commits erstellt hast, wird ein `git push` mit einer Meldung wie `fetch first` abgelehnt.

1. Lade die Änderungen vom Remote-Repository und setze deine lokalen Commits darauf:

```bash
git pull --rebase origin main
```

2. Falls Git einen Konflikt meldet, öffne die betroffenen Dateien und behebe die Konflikte. Anschließend die gelösten Dateien zur Staging Area hinzufügen, z. B.:

```bash
git add README.md
```

3. Die Rebase fortsetzen:

```bash
git rebase --continue
```

4. Wiederhole Schritt 2 und 3, bis die Rebase abgeschlossen ist (falls mehrere Konflikte auftreten).

5. Zum Schluss die Änderungen auf GitHub hochladen:

```bash
git push origin main
```

> **Hinweis:** Wenn `git pull --rebase` ohne Konflikte durchläuft, sind die Schritte `git add` und `git rebase --continue` nicht erforderlich. In diesem Fall kannst du direkt `git push origin main` ausführen.
