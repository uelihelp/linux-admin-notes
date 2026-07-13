# Firefox: RAM-Verbrauch reduzieren

## Voraussetzungen

Öffne einen neuen Tab und rufe `about:config` auf.

## Einstellungen

Suche nach:

`browser.tabs.unloadOnLowMemory`

und setze den Wert auf:

`true`

Suche anschließend nach:

`browser.tabs.min_inactive_duration_before_unload`

Der Wert wird in Millisekunden angegeben.

Beispiel:

- `600000` = 10 Minuten
- `1800000` = 30 Minuten
- `3600000` = 1 Stunde

Diese Einstellung gibt an, wie lange ein Tab inaktiv sein muss, bevor Firefox ihn aus dem Arbeitsspeicher entladen darf.

Der Tab bleibt erhalten und wird beim erneuten Anklicken automatisch neu geladen.

## Speicherverwaltung prüfen

Öffne einen neuen Tab und rufe `about:unloads` auf.

Dort kannst du sehen,

- welche Tabs Firefox als Nächstes entladen würde,
- wie die Priorität berechnet wird,
- und das Entladen von Tabs manuell auslösen.
