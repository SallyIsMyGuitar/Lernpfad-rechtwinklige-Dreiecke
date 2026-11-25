# Lernpfad: Rechtwinklige Dreiecke

Interaktiver Lernpfad für die **9. Jahrgangsstufe, Wahlpflichtfächergruppe I (Mathematik, Realschule Bayern)**, Kapitel 5 „Rechtwinklige Dreiecke“ (LehrplanPLUS M9, Lernbereich 3). Die Schülerinnen und Schüler erarbeiten das Kapitel selbstständig, entdecken Regeln selbst und üben auf ihrem Niveau.

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
| 1 | Den Satz des Pythagoras entdecken | fertig |
| 2 | Seitenlängen berechnen (Hypotenuse, Kathete, Einheiten, Lage des rechten Winkels) | fertig |
| 3 | Umkehrung: Rechtwinkligkeit prüfen | fertig |
| 4 | Satz des Pythagoras in ebenen Figuren | fertig |
| 5 | Funktionale Abhängigkeiten und Extremwerte | geplant |
| 6 | Pythagoras in Körpern | geplant |
| 7 | Koordinatensystem: Strecken, Betrag, Rechtwinkligkeit | geplant |
| 8 | Streckenlänge in Abhängigkeit von x | geplant |
| 9 | Abschluss-Check | geplant |

Noch offen: Sinus, Kosinus und Tangens (Lehrplan), eine Auffrischung der quadratischen Ergänzung vor Station 5 und ein Punkteschema für den Abschluss-Check.

## Nutzung

**Lokal:** `index.html` im Browser öffnen.

**Über GitHub Pages:** im Repository unter *Settings → Pages* den Branch `main` und den Ordner `/ (root)` auswählen. Die Seite ist danach unter `https://<benutzername>.github.io/<repository>/` erreichbar.

**Lehrkraft-Ansicht:** Mit `?lehrer=1` an der Adresse (`…/index.html?lehrer=1`) sind alle Stationen freigeschaltet. Auf der Übersicht steht dann eine Tabelle mit den gültigen Kontrollcodes je Station und Punktzahl für ein wählbares Datum.

**Geteilte iPads:** Auf der Übersicht gibt es den Button „Fortschritt zurücksetzen“ (mit Sicherheitsabfrage). Er löscht alle gespeicherten Daten auf dem Gerät.

**Fortsetzen:** Erledigte Schritte einer Station werden gespeichert. Nach dem Neuladen geht es beim nächsten offenen Schritt weiter; erledigte Schritte lassen sich erneut ansehen.

## Erklärvideos einbinden

Ganz oben im Skript der Datei steht die Konfiguration `VIDEOS`. Pro Station kann eine YouTube-Video-ID eingetragen werden. Das Video wird dann datenschutzfreundlich (`youtube-nocookie.com`) eingebettet. Ohne ID erscheint ein Button mit einer YouTube-Suche zum angegebenen Suchbegriff.

```js
const VIDEOS={
  s1:{videoId:'XXXXXXXXXXX',query:'Satz des Pythagoras Herleitung'},
  // s2, s3, s4 analog
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

Alle Aufgaben, Merkkästen und Texte sind eigene Formulierungen. Es sind keine Inhalte aus Schulbüchern oder Leistungsnachweisen übernommen.
