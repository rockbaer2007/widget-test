# UGSo Widget Test

Referenzpaket für die deklarative Widget-Schnittstelle 0.1 von [HA Grafik Visual Studio](https://github.com/rockbaer2007/ugso-ha-mqtt-addons/tree/master/ha_grafik_visual_studio). Das Paket enthält ein **Status Label** mit bearbeitbarem Text und einem geprüften SVG-Palettenbild. Es führt keinen eigenen Code aus. Das getrennte [Tools-Test-Repository](https://github.com/rockbaer2007/tools-test) prüft die Tool-Schnittstelle.

## Funktionstest

1. Lade `widget-test-0.1.0.wg.zip` aus dem [Release v0.1.0](https://github.com/rockbaer2007/widget-test/releases/tag/v0.1.0) herunter oder erstelle es mit `python build.py` neu.
2. Installiere die Datei unter **Einstellungen → Widget-Pakete** im Studio und lade die App neu.
3. Prüfe, ob **UGSo Widget Test** in der Palette erscheint. Füge **Status Label** ein, ändere den Text unter **Inhalt** und prüfe ihn im Editor und in der Runtime.
4. Solange das Widget in einem Projekt verwendet wird, muss **Entfernen** gesperrt sein. Nach dem Löschen aller Instanzen darf das Paket entfernt werden.

Quelle: `package/manifest.json` und `package/icons/widget-test.svg`. `dist/` enthält die fertige Testdatei. Der aktuelle Importer nimmt `.wg.zip` an; die spätere Endung `.wg` ist noch nicht implementiert. Weitere Regeln stehen in der [Widget-Schnittstellenbeschreibung](https://github.com/rockbaer2007/ugso-ha-mqtt-addons/blob/master/ha_grafik_visual_studio/docs/widget-rules.md).

## English

This is a reference package for HA Grafik Visual Studio's declarative widget API 0.1. Download `widget-test-0.1.0.wg.zip` from [release v0.1.0](https://github.com/rockbaer2007/widget-test/releases/tag/v0.1.0), or rebuild it with `python build.py`. Install it under **Settings → Widget packages** and reload the app. The **UGSo Widget Test** palette set should contain **Status Label**. Edit its text and check the editor and runtime. Removal must be blocked while any project uses the widget. The current importer accepts `.wg.zip`; `.wg` is planned for a later version.
