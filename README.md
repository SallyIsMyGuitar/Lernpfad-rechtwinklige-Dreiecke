# Lernpfad: Rechtwinklige Dreiecke

Interaktiver Lernpfad für die **9. Jahrgangsstufe, Wahlpflichtfächergruppe I (Mathematik, Realschule Bayern)**, Kapitel 5 „Rechtwinklige Dreiecke“ (LehrplanPLUS M9, Lernbereich 3). Die Schülerinnen und Schüler erarbeiten das Kapitel selbstständig, entdecken Regeln selbst und üben auf ihrem Niveau.

> **Status: Beta-Phase – in Prüfung.** Alle Stationen werden derzeit von der Lehrkraft fachlich und didaktisch geprüft (u. a. Abgleich mit dem LehrplanPLUS) und sind noch **nicht für den Unterricht freigegeben**. Die Erklärvideos fehlen noch vollständig (siehe „Noch offen“).

Die Seite besteht aus **einer einzigen Datei** (`index.html`) ohne Abhängigkeiten, Build-Schritte oder Server. Sie läuft im Browser, auch auf dem iPad.

## Aufbau jeder Station

1. **Entdecken:** interaktives Experiment oder geführte Schritte, optional mit Erklärvideo (YouTube).
2. **Regel formulieren:** Lückentext oder Auswahlfragen mit direkter Rückmeldung.
3. **Merkheft-Eintrag:** gelb markierter Kasten mit Beispielen, der ins Merkheft abgeschrieben wird (Bestätigung per Häkchen).
4. **Üben:** drei Niveaus (leicht, standard, plus) mit zufällig erzeugten Aufgaben, Tipps und Lösungsweg. Eine Aufgabe zählt nur, wenn sie ohne angezeigten Lösungsweg gelöst wird (Auswahlaufgaben im 1. Versuch, Rechenaufgaben spätestens im 2. Versuch).
5. **Exit-Ticket:** drei Fragen aus einem Fragen-Pool in zufälliger Reihenfolge, je ein Versuch. Die Lösungen erscheinen erst in der Auswertung, bei einer Wiederholung kommen neue Fragen. Ab 2 von 3 richtig erscheint eine Check-in-Karte mit Datum, geübtem Niveau und Kontrollcode, und die nächste Station wird freigeschaltet.

Im Kopf der Seite gibt es eine Übersicht aller Merkheft-Einträge zum Nachlesen, Drucken oder als PDF sichern.

## Stationen

| Nr. | Station | Stand |
|---|---|---|
| 1 | Den Satz des Pythagoras entdecken | Beta – in Prüfung |
| 2 | Seitenlängen berechnen (Hypotenuse, Kathete, Einheiten, Lage des rechten Winkels) | Beta – in Prüfung |
| 3 | Umkehrung: Rechtwinkligkeit prüfen | Beta – in Prüfung |
| 4 | Satz des Pythagoras in ebenen Figuren | Beta – in Prüfung |
| 5 | Funktionale Abhängigkeiten und Extremwerte (Strecken und Flächen mit wandernden Punkten, Auffrischung quadratische Ergänzung) | Beta – in Prüfung |
| 6 | Pythagoras in Körpern (Quader, Würfel, gerade quadratische Pyramide) | Beta – in Prüfung |
| 7 | Koordinatensystem: Strecken als Betrag eines Vektors, Rechtwinkligkeit von Dreiecken prüfen | Beta – in Prüfung |
| 8 | Streckenlänge in Abhängigkeit von x (Punkte P<sub>n</sub> auf einer Geraden, fester Punkt Q, kürzeste Strecke per quadratischer Ergänzung) | Beta – in Prüfung |
| 9 | Abschluss-Check | Beta – in Prüfung |

**Abschluss-Check (Station 9):** 12 zufällig erzeugte Aufgaben aus den Stationen 1–8 mit insgesamt 18 Punkten (je 1 oder 2 Punkte), ein Versuch pro Aufgabe, die Rückmeldung kommt erst in der Auswertung. Bestanden ab 9 Punkten (50 %). Die Auswertung zeigt die Punkte je Station mit Wiederholungsempfehlung und alle Aufgaben mit Lösungsweg. Ab 9 Punkten erscheint die Check-in-Karte mit Kontrollcode, sonst kann der Check mit neuen Aufgaben wiederholt werden. Keine Note.

**Legende Stand:** *Beta – in Prüfung* = inhaltlich umgesetzt, aber noch nicht von der Lehrkraft geprüft und freigegeben. Nach der Prüfung wird der Stand auf *freigegeben* gesetzt.

### Noch offen

- [ ] **Prüfung und Freigabe** aller Stationen 1–9 (fachliche Richtigkeit, Lehrplanbezug LehrplanPLUS M9, Niveau der Aufgaben)
- [ ] **Erklärvideos:** Für die Stationen 1–8 sind noch keine passenden Erklärvideos eingetragen (in `VIDEOS` steht überall `videoId:null`). Aktuell erscheint nur ein Button mit einer YouTube-Suche. Passende Videos müssen ausgewählt, geprüft und eingetragen werden (siehe „Erklärvideos einbinden“).
- [ ] Sinus, Kosinus und Tangens (Lehrplan)

## Nutzung

**Lokal:** `index.html` im Browser öffnen.

**Über GitHub Pages:** im Repository unter *Settings → Pages* den Branch `main` und den Ordner `/ (root)` auswählen. Die Seite ist danach unter `https://<benutzername>.github.io/<repository>/` erreichbar.

**Lehrkraft-Ansicht:** Mit `?lehrer=1` an der Adresse (`…/index.html?lehrer=1`) sind alle Stationen freigeschaltet. Auf der Übersicht steht dann eine Tabelle mit den gültigen Kontrollcodes je Station und Punktzahl für ein wählbares Datum (für den Abschluss-Check je Punktzahl von 9 bis 18).

**Geteilte iPads:** Auf der Übersicht gibt es den Button „Fortschritt zurücksetzen“ (mit Sicherheitsabfrage). Er löscht alle gespeicherten Daten auf dem Gerät.

**Fortsetzen:** Erledigte Schritte einer Station werden gespeichert. Nach dem Neuladen geht es beim nächsten offenen Schritt weiter; erledigte Schritte lassen sich erneut ansehen.

## Erklärvideos einbinden

Ganz oben im Skript der Datei steht die Konfiguration `VIDEOS`. Pro Station kann eine YouTube-Video-ID eingetragen werden. Das Video wird dann datenschutzfreundlich (`youtube-nocookie.com`) eingebettet. Ohne ID erscheint ein Button mit einer YouTube-Suche zum angegebenen Suchbegriff.

```js
const VIDEOS={
  s1:{videoId:'XXXXXXXXXXX',query:'Satz des Pythagoras Herleitung'},
  // s2 bis s8 analog
};
```

## Datenschutz

- Es werden keine Namen oder Konten abgefragt und keine Daten an einen Server gesendet.
- Der Fortschritt (Station, erledigte Schritte, geübtes Niveau, Ergebnis, Datum, Kontrollcode) liegt nur im `localStorage` des jeweiligen Browsers und lässt sich auf der Übersicht löschen.
- Der Kontrollcode auf der Check-in-Karte ist ein Plausibilitätscheck, kein Manipulationsschutz.
- Externe Inhalte werden nur beim Klick auf den YouTube-Link oder bei eingetragener Video-ID geladen.

## Technik

- Reines HTML, CSS und JavaScript in einer Datei, keine Bibliotheken.
- Aufgaben werden im Browser zufällig erzeugt, Lösungswege werden aus denselben Werten berechnet.
- Grafiken sind SVG und werden im Code erzeugt.

## Hinweise zu den Inhalten

Die Schreibweisen folgen dem [Zeichenkatalog des ISB für Mathematik an der Realschule, Jgst. 5–10](https://www.lehrplanplus.bayern.de/fm/71/RS_M_5_10_Zeichenkatalog.pdf) (Stand 12.07.2022):

- rechter Winkel in Zeichnungen: kleiner Winkelbogen mit einem Punkt in der Mitte
- Strecke: AB mit Strich darüber, Länge der Strecke: |AB| mit Strich über AB (AB ohne Strich bezeichnet die Gerade)
- Quadratwurzel mit Wurzelstrich über dem Radikanden, Brüche mit Bruchstrich
- Winkelmaße α, β, γ; Umfang u; Flächeninhalt A
- Vektoren mit Pfeil darüber, Koordinaten als Spaltenvektor; Punkte P(x | y)
- wandernde Punkte mit Index n (P<sub>n</sub>, Q<sub>n</sub>); Schrägbilder mit Verzerrungswinkel 45° und Verkürzungsfaktor ½, verdeckte Kanten gestrichelt


Alle Aufgaben, Merkkästen und Texte sind eigene Formulierungen. Es sind keine Inhalte aus Schulbüchern oder Leistungsnachweisen übernommen.
