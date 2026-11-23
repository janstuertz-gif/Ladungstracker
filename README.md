# Ladelog

Zeichnet auf, wann dein Handy lädt, und zeigt es als Diagramm mit Auswertung.
Gedacht, um „Intelligentes Laden“ zu testen: Hört das Handy bei 100 % wirklich auf zu laden
und macht erst unter 95 % weiter?

## APK bauen (wie bei deinen anderen Apps)
1. Den gesamten Inhalt dieses Ordners (auch `.github`) in ein **neues** GitHub-Repo hochladen.
2. Actions → „Build APK“ → fertigen Lauf öffnen → Artifact **Ladelog-APK** → APK installieren.

## Benutzen
1. App öffnen, Benachrichtigungen erlauben, „Akku-Optimierung ausschalten“ tippen.
   In den Handy-Einstellungen für die App außerdem Autostart / Hintergrundaktivität erlauben.
2. Die Aufzeichnung startet automatisch (Benachrichtigung „Ladelog läuft“).
3. „Intelligentes Laden“ einschalten, Handy auf 100 % laden und am Kabel lassen (am besten über Nacht).
4. Danach die App öffnen.

## So liest du das Ergebnis
- Blaue Linie = Akkustand. Grün = lädt. Orange = am Kabel, aber lädt nicht. Rot = keine Daten.
- Unter „Test“ steht, wann das Laden gestoppt hat und bei welchem Akkustand es wieder gestartet ist.
- „Ø mA“ ist der durchschnittliche Ladestrom der Phase. Zeigt ein grüner Abschnitt etwa 0 mA, fließt kaum Strom.
  (Manche Handys melden mA statt µA. Sind alle Werte 1000-mal zu klein, bitte melden.)
- Rote Lücken heißen: In der Zeit lief die Aufzeichnung nicht (z. B. vom Handy beendet).
- „Auswertung kopieren“ und „Rohdaten (24 h) kopieren“ liefern Text zum Weitergeben.

Gemessen wird bei jeder Änderung und mindestens jede Minute. Die Daten bleiben nur auf dem Handy.
