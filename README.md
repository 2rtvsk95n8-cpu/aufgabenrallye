# Aufgabenrallye – Technische Mathematik

Web-App für den Unterricht mit dem Arbeitsheft „Metalltechnik – Technische Mathematik Grundbildung“, Seiten 5–112.
Die Schüler scannen einen QR-Code, geben ihre Ergebnisse ein und bekommen für jedes richtige Ergebnis Punkte. Am Beamer läuft ein Live-Ranking.

Enthalten sind 61 Kapitel in 10 Bereichen mit 669 prüfbaren Ergebnissen:
Grundrechnen, Gleichungen & Formeln, Längen & Winkel, Flächen, Volumen & Masse, Kräfte & Mechanik, Bewegung, Druck & Hydraulik, Elektrotechnik und Praxisaufgaben.

## Online stellen (GitHub Pages)

1. Auf GitHub oben rechts **+ → New repository** wählen.
   Name: `aufgabenrallye` · **Public** · „Create repository“.
2. Auf der neuen Seite **„uploading an existing file“** anklicken.
   Diese Dateien hineinziehen: `index.html`, `lehrer.html`, `README.md`, `HINWEISE-LIZENZEN.md`.
   Unten **„Commit changes“** klicken.
3. **Settings → Pages** öffnen.
   Bei *Source* „Deploy from a branch“ auswählen, bei *Branch* **main** und **/(root)** einstellen und **Save** klicken.
4. Nach 1–2 Minuten erscheint oben auf der Pages-Seite die Adresse, zum Beispiel
   `https://2rtvsk95n8-cpu.github.io/aufgabenrallye/`

## Im Unterricht

| Wer | Adresse |
|---|---|
| Lehrkraft (Beamer) | `https://2rtvsk95n8-cpu.github.io/aufgabenrallye/lehrer.html` |
| Schüler | QR-Code vom Beamer scannen oder Startseite öffnen und Raumcode eingeben |

- **Aufgaben auswählen:** In der Lehrer-Ansicht unter „Aufgaben dieser Runde“ auf **Auswählen …** klicken.
  Dort lassen sich ganze Bereiche („alle an/aus“), einzelne Kapitel oder über **▾** einzelne Aufgaben wählen. Mit **Übernehmen** erscheint die Auswahl sofort auf allen Handys.
- **Der Raum bleibt erhalten.** Lädt man die Lehrer-Seite neu, gelten derselbe Raumcode und derselbe QR-Code weiter. „Neuen Raum erstellen“ erzeugt einen neuen.
- **Neue Runde** setzt alle Punkte auf 0, der Raum bleibt.
- **Hilfen freigeben / Ergebnisse freigeben** gilt sofort auf allen Handys.
- **Hinweis an alle** blendet einen Text auf allen Handys ein. Wer das Feld leer sendet, blendet den Hinweis wieder aus.
- **×** neben einem Namen entfernt die Person, zum Beispiel bei einem unpassenden Namen.

### Punkte
- Jedes Ergebnis bringt 10 Punkte, eine Formel-Auswahl (Umstellen von Formeln) 5 Punkte. Ranking und Höchstpunktzahl richten sich nach der aktuellen Auswahl.
- Volle Punktzahl gibt es für ein richtiges Ergebnis beim ersten Versuch.
- Ein Fehlversuch kostet 20 % der Punkte. Hilfe 1 kostet ebenfalls 20 %, Hilfe 2 weitere 30 %.
- Mindestens 20 % der Punkte bleiben immer.
- Ungültige Eingaben (keine Zahl) kosten nichts.

### Eingaben
- Zahlen mit Komma oder Punkt, Brüche als `3/4` oder `2 3/8`, Winkel als `37°50'` oder Dezimalzahl, Verhältnisse als `1:4`, kleine Zahlen als `1,74e-3`.
- Beim Erweitern und Kürzen muss der Bruch genau in der verlangten Form eingegeben werden.

### Toleranzen
- Rechenergebnisse dürfen je nach Aufgabe etwa 0,2–1,5 % abweichen (Rundung, π = 3,14). Bei Prüfmaßen und Umrechnungen ist die Toleranz sehr klein.
- Bei zeichnerischen Lösungen und Diagrammwerten gilt eine größere Spanne (3–5 %).
- Wo das Buch mit g ≈ 10 m/s² rechnet, zählt auch das Ergebnis mit g = 9,81 m/s².
- Bei Pyramidenstumpf und Kegelstumpf zählen sowohl das Ergebnis der Näherungsformel (Buch) als auch das exakte Ergebnis.
  Beim Kegelstumpf: ≈ 1,6 m³ mit Näherung, ≈ 1,19 m³ exakt.
- Für Tabellenbuch-Werte gilt jeweils eine kleine Spanne.

## Vor der ersten Stunde testen

Lehrer-Seite im Schul-WLAN öffnen und prüfen, ob unter den Einstellungen bei mindestens einem Server ein **✓** steht. Danach mit einem Handy beitreten.
Die App nutzt drei kostenlose öffentliche Server gleichzeitig: HiveMQ (Port 8884), EMQX (Port 8084) und Eclipse (Port 443).
Steht überall „–“, blockiert vermutlich die Schul-Firewall die Server. Dann die IT bitten, diese Server freizugeben.

## Datenschutz

Auf den öffentlichen Servern sind Spitzname und Punktestand für jeden sichtbar, der den Raumcode kennt.
Deshalb nur **Vornamen oder Spitznamen** verwenden und keine weiteren persönlichen Daten.
Alles andere bleibt auf dem jeweiligen Gerät: Eingaben, Fortschritt und Lösungen.
Die Seite lädt keine externen Schriften und keine Tracker.

## Hinweise

- Die Ergebnisse werden auf dem Handy geprüft. Die Lösungen liegen dort verschlüsselt vor, sind für sehr findige Schüler aber auslesbar.
- Die Seite funktioniert nur online über die GitHub-Pages-Adresse. In einer Vorschau oder als lokale Datei zeigt sie einen Hinweis statt des QR-Codes.
