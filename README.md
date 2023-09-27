![Toptipper](/lmo/help/media/addons.png)
# Toptipper

| 1. **Systemvoraussetzung**<br/>2. **Zur Erklärung der Dateien**<br/>3. **Download**         |                                    |
|:------------------------------------------------------------------------------------------- | ---------------------------------- |
| Das Addon TopTipper gibt Ihnen eine Anzeige<br>des Tabellenstandes im Tippspiel des LMO's.) | ![](/lmo/help/media/toptipper.png) |



---

## Systemvoraussetzung

- Lauffähiger LMO 4 ab Beta 3 mit Tippspiel

---

## Zur Erklärung der Dateien

Der Inhalt des Downloads besteht aus 4 Dateien.



**toptipper.php**

Addon Datei<br>
befindet sich im Ordner 'addon/tipp/'



**kal.tip**

befindet sich im Ordner 'config/tipp/'<br>
Ist für die Konfiguration und kann beliebig umbenannt werden. Hauptsache die Dateiendung ***.tipp** bleibt bestehen und der neue Name wird auch beim einbinden berücksichtigt.  

- Der Inhalt der Datei besteht aus  

| [config]          |                                                                                      |
| ----------------- | ------------------------------------------------------------------------------------ |
| modus=1           | **// Modus auf 1 lassen kann man vielleicht noch mal gebrauchen**                    |
| anzahl_tipper=10  | **// Anzahl der Tipper in der Anzeige**                                              |
| all=0             | **// 0 oder 1, 0 zeigt das file (eine Liga), 1 die gesamt.aus (bei mehreren Ligen)** |
| file=erg_dfb.l98  | **// eure Liga**                                                                     |
| template=standard | **// Template Name ohne die Endung (.tpl.php)**                                      |



**standard.tpl.php**

befindet sich im Ordner 'template/tipp/'<br>
Das Template kann beliebig erstellt werden. Verfügbare Platzhalter sind derzeit:
| Platzhalter      | Beschreibung                            |
| ----------------:|:--------------------------------------- |
| `<!--URLTipp-->` | **Der Link zum Tippspiel**              |
| `<!--gotoTipp-->`| **Der Name für den Link zum Tippspiel** |
| `<!--URLLMO-->`  | **Der Link zum LMO**                    |
| `<!--gotoLMO-->` | **Der Name für den Link zum LMO**       |
| `<!--Platz-->`   | **Die Platzierung der Tipper**          |
| `<!--Name-->`    | **Der Name der Tipper**                 |
| `<!--Punkte-->`  | **Die Punkte der Tipper**               |



**tipp.php**

befindet sich direkt im Root_Verzeichniss Ihres LMO's.

Dient zum Einbinden des ganzen Scriptes (Inhalt anpassen)

- Beispiel:

```php
<?php
  $multi="kal";  //in diesem Fall wird die von euch angepasste Datei kal.tip eingebunden.
  require(dirname(__FILE__).'/init.php');
  include(PATH_TO_ADDONDIR."/tipp/toptipper.php");
?>
```

---

## Download

- [Download](https://github.com/henshingly/Toptipper/tags)

---
