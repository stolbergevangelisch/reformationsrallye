# oh! Orange -- Rallye zur Reformation

Die Webseite ist eine statische Browser-Rallye. Sie braucht keine Installation, Anmeldung, Datenbank oder externen Schriften. Jede Station hat einen eigenen QR-Code. Der Fortschritt bleibt auf demselben Gerät im selben Browser gespeichert. Die zehn Stationen werden nacheinander freigeschaltet. Falsche Antworten können beliebig oft wiederholt werden.

## Auf GitHub Pages veröffentlichen

1. ZIP-Datei entpacken.
2. Im GitHub-Konto `stolbergevangelisch` ein neues öffentliches Repository mit dem Namen **reformationsrallye** anlegen.
3. Die Dateien aus diesem Ordner direkt in das Hauptverzeichnis des Repositorys hochladen. Wichtig: `index.html` muss direkt dort liegen, nicht in einem Unterordner. Die Datei `.nojekyll` ist optional, falls sie im Dateidialog verborgen ist.
4. Änderungen auf dem Branch `main` speichern (Commit).
5. Unter **Settings → Pages** bei **Build and deployment** die Quelle **Deploy from a branch** wählen. Branch **main**, Ordner **/(root)** auswählen und speichern.
6. Nach erfolgreicher Bereitstellung diese Adresse öffnen: https://stolbergevangelisch.github.io/reformationsrallye/
7. Vor dem Drucken alle QR-Codes mit einem Smartphone testen. Die Codes in der Präsentation sind bereits für genau diese Adresse und `?station=1` bis `?station=10` angelegt. Bei einem anderen Repositorynamen müssen die QR-Codes neu erstellt werden.

GitHub-Anleitung: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Lokal ansehen

`index.html` im Browser öffnen. Für einen zuverlässigen Test von Speicherung und QR-Adressen einen lokalen Webserver oder die veröffentlichte HTTPS-Adresse verwenden. Ein Wechsel zwischen verschiedenen Browsern oder dem privaten und normalen Modus übernimmt den Fortschritt nicht. Ohne verfügbaren Browserspeicher erscheint ein Hinweis; dann die Seite geöffnet lassen und mit „Weiter“ fortfahren.

## Fragen ändern

Alle Texte stehen in `data.js`: `q` ist die Frage, `a` enthält die vier Antworten, `correct` die richtige Antwort (0 = A, 1 = B, 2 = C, 3 = D), `letters` die Papier-Lösungsbuchstaben. Der Buchstabe bei der richtigen Antwort ergibt zusammen mit den übrigen Stationen FINKENBERG. `hint` führt zur nächsten Station. Bei Änderung der Antwortreihenfolge auch `correct` und `letters` anpassen.

**Noch offen:** Die Stufenzahl bei Station 4 steht vorläufig auf 23. Sobald sie feststeht, die Antwort in `data.js` und auf Folie 4 ändern. Die QR-Codes bleiben dabei unverändert.

Die Präsentation enthält zehn A4-Querformat-Seiten mit weißem Hintergrund, schwarzer Schrift, Logo, Frage, vier Antworten mit Lösungsbuchstaben, Fundorthinweis und QR-Code. Für die Papier-Rallye den Buchstaben neben der gewählten Antwort notieren. Hinweise stehen auf dem Papier direkt sichtbar. Die richtigen Antworten, Orte und Buchstaben stehen in den PowerPoint-Notizen und in `LOESUNGEN.md`.

## Speicher und Datenschutz

Die App sendet keine Antworten und nutzt keine Analysewerkzeuge. Sie speichert ausschließlich die Anzahl der gelösten Stationen lokal im Browser. Der Hosting-Anbieter verarbeitet bei Seitenaufrufen die üblichen Verbindungsdaten. Für den Einsatz kann die Gemeinde die Seite in ihre vorhandenen Datenschutz- und Anbieterinformationen einbinden.

Die Reihenfolge steuert den Spielablauf. Da alle Lösungen im ausgelieferten Quelltext stehen, ist die Webseite kein gegen Manipulation geschütztes Prüfungssystem.
