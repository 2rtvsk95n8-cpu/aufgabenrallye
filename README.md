# Aufgabenrallye – Volumen, Dichte & Masse

Web-App für den Unterricht in Technischer Mathematik (Arbeitsblätter S. 47–49: Volumenberechnung II, Masseberechnung I).
Die Schüler scannen einen QR-Code, geben ihre Ergebnisse ein und bekommen für jedes richtige Ergebnis Punkte. Am Beamer läuft ein Live-Ranking.

## Online stellen (GitHub Pages)

1. Auf GitHub oben rechts **+ → New repository** wählen.
   Name: `rechenrallye` · **Public** · „Create repository“.
2. Auf der neuen Seite **„uploading an existing file“** anklicken.
   Diese Dateien hineinziehen: `index.html`, `lehrer.html`, `README.md`, `HINWEISE-LIZENZEN.md`.
   Unten **„Commit changes“** klicken.
3. **Settings → Pages** öffnen.
   Bei *Source* „Deploy from a branch“ auswählen, bei *Branch* **main** und **/(root)** einstellen und **Save** klicken.
4. Nach 1–2 Minuten erscheint oben auf der Pages-Seite die Adresse, zum Beispiel
   `https://2rtvsk95n8-cpu.github.io/rechenrallye/`

## Im Unterricht

| Wer | Adresse |
|---|---|
| Lehrkraft (Beamer) | `https://2rtvsk95n8-cpu.github.io/rechenrallye/lehrer.html` |
| Schüler | QR-Code vom Beamer scannen oder Startseite öffnen und Raumcode eingeben |

- **Der Raum bleibt erhalten.** Lädt man die Lehrer-Seite neu, gelten derselbe Raumcode und derselbe QR-Code weiter. „Neuen Raum erstellen“ erzeugt einen neuen.
- **Neue Runde** setzt alle Punkte auf 0, der Raum bleibt.
- **Hilfen freigeben / Lösungswege freigeben** gilt sofort auf allen Handys.
- **Hinweis an alle** blendet einen Text auf allen Handys ein. Wer das Feld leer sendet, blendet den Hinweis wieder aus.
- **×** neben einem Namen entfernt die Person, zum Beispiel bei einem unpassenden Namen.

### Punkte (190 insgesamt)
- Volle Punktzahl gibt es für ein richtiges Ergebnis beim ersten Versuch.
- Ein Fehlversuch kostet 20 % der Aufgabenpunkte. Hilfe 1 kostet ebenfalls 20 %, Hilfe 2 weitere 30 %.
- Mindestens 20 % der Punkte bleiben immer.
- Ungültige Eingaben (keine Zahl) kosten nichts.

### Toleranzen
- Rechenergebnisse dürfen etwa 1,5–2 % abweichen (Rundung, π = 3,14).
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
