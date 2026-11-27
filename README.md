# Aufgabenrallye – Mathe-Arbeitsheft und Fachbuch SHK

Web-App für den Unterricht. Die Schüler scannen einen QR-Code, bearbeiten die ausgewählten Aufgaben, sammeln Punkte und helfen sich gegenseitig über die **Hilfeampel**.

- **Mathe-Arbeitsheft** „Metalltechnik – Technische Mathematik Grundbildung“: 61 Kapitel, 669 automatisch geprüfte Ergebnisse.
- **Fachbuch SHK Lernfelder 1–15**: 71 Kapitel mit 766 Fragen „Zur Wiederholung“, 417 „Zur Vertiefung“ und 305 „Zur Berechnung“.
- Alle Seitenzahlen gelten für die neueren Auflagen der Schüler (Lösungsheft/6. Auflage + 2).

## Online stellen (GitHub Pages)

Die Seite läuft unter `https://2rtvsk95n8-cpu.github.io/aufgabenrallye/`.

## Im Unterricht

| Wer | Adresse |
|---|---|
| Lehrkraft (Beamer) | `https://2rtvsk95n8-cpu.github.io/aufgabenrallye/lehrer.html` |
| Schüler | QR-Code vom Beamer scannen oder Startseite öffnen und Raumcode eingeben |

- **Aufgaben auswählen:** Unter „Aufgaben dieser Runde“ auf **Auswählen …** klicken. Oben zwischen **Mathe-Arbeitsheft** und **Fachbuch SHK** wechseln (beides lässt sich mischen).
  Wählbar sind ganze Bereiche bzw. Lernfelder, Kapitel, beim Fachbuch die Blöcke W/V/B und über **▾** einzelne Aufgaben.
- **Namen:** Schüler geben einmal ihren richtigen Vornamen ein (sieht nur die Lehrkraft) und wählen ein Pseudonym aus einer festen Liste. Jede/r entscheidet selbst, ob in der Klasse der Vorname oder das Pseudonym erscheint.
  Vorname und Punkte werden verschlüsselt übertragen; nur der Lehrer-Browser kann sie lesen.
- **Beamer:** QR-Code, **Top 5** und **Hilfeampel**. Mehr Leistungsdaten erscheinen dort nicht.
- **Lehreransicht (privat):** Vornamen, Punkte, Hilfen, Ampel und die Antworten jeder Person. Nicht am Beamer öffnen.
- **Hilfeampel:** Rot = Hilfe benötigt (selbst angetippt oder nach drei Fehlversuchen), Gelb = in Arbeit, Grün = erledigt. Wer überall Grün hat, bekommt einen Hinweis, wer noch Hilfe braucht.
- **Fachbuch-Paket:** Fragentexte und Musterlösungen liegen **nicht** in diesem Repository. Die Lehrkraft lädt die Datei `Fachbuch-Paket_SHK_LF1-15.json` in der privaten Lehreransicht. Die App verteilt dann die Fragen im Raum, die Musterlösungen erst nach „Lösungen anzeigen“.
- **Der Raum bleibt erhalten.** Lädt man die Lehrer-Seite neu, gelten derselbe Raumcode und derselbe QR-Code weiter. „Neuen Raum erstellen“ erzeugt einen neuen.
- **Neue Runde** setzt alle Punkte auf 0, der Raum bleibt.
- **Hilfen freigeben / Lösungen anzeigen** gilt sofort auf allen Handys.
- **Hinweis an alle** blendet einen Text auf allen Handys ein. Wer das Feld leer sendet, blendet den Hinweis wieder aus.
- **×** neben einem Namen entfernt die Person, zum Beispiel bei einem unpassenden Namen.

### Punkte
- Fachbuch-Fragen: „Fertig“ = 5 P (jede Hilfe −1 P). Nach der Lösungsfreigabe prüfen die Schüler selbst: richtig +5 P, teilweise +2 P.
- Mathe: Jedes Ergebnis bringt 10 Punkte, eine Formel-Auswahl (Umstellen von Formeln) 5 Punkte. Die Punkte richten sich nach der aktuellen Auswahl.
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

Im Raum sichtbar sind nur der angezeigte Name (Pseudonym oder freiwillig der Vorname), die Ampelfarben und die Top 5.
Der richtige Vorname, die Punkte und die Antworten werden mit dem Schlüssel des Lehrer-Browsers verschlüsselt.
Der Schlüssel liegt nur in diesem Browser. Ein neuer Browser oder Rechner bedeutet einen neuen Raum.
Alles andere bleibt auf dem jeweiligen Gerät: Eingaben, Fortschritt und Lösungen.
Die Seite lädt keine externen Schriften und keine Tracker.

## Hinweise

- Die Ergebnisse werden auf dem Handy geprüft. Die Lösungen liegen dort verschlüsselt vor, sind für sehr findige Schüler aber auslesbar.
- Die Seite funktioniert nur online über die GitHub-Pages-Adresse. In einer Vorschau oder als lokale Datei zeigt sie einen Hinweis statt des QR-Codes.
