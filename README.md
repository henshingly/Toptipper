[<img src="https://www.vest-sport.de/forum_files/addon.svg">](https://www.vest-sport.de/forum)
# Toptipper
[![GitHub release](https://img.shields.io/github/release/henshingly/Toptipper?include_prereleases=&sort=semver&color=blue)](https://github.com/henshingly/Toptipper/releases/)
[![download-badge](https://img.shields.io/github/downloads/henshingly/Toptipper/total.svg?style=flat-square "Download status")](https://github.com/henshingly/Toptipper/releases/latest "Download status")
[![Donate](https://img.shields.io/badge/-Buy%20me%20a%20coffee-brown.svg)](https://paypal.me/LMOforum)

## Deutsch

| 1. **Systemvoraussetzung**<br/>2. **Zur Erklärung der Dateien**<br/>3. **Download**         |                                    |
|:------------------------------------------------------------------------------------------- | ---------------------------------- |
| Das Addon TopTipper gibt Ihnen eine Anzeige<br>des Tabellenstandes im Tippspiel des LMO's.) | ![](/lmo/help/media/toptipper.png) |


---

### Systemvoraussetzung

- Lauffähiger LMO 4 ab Beta 3 mit Tippspiel

---

### Zur Erklärung der Dateien

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
  $multi = "kal";  //in diesem Fall wird die von euch angepasste Datei kal.tip eingebunden.
  require(dirname(__FILE__) . '/init.php');
  include(PATH_TO_ADDONDIR . "/tipp/toptipper.php");
?>
```

---

### Download

- [Download](https://github.com/henshingly/Toptipper/tags)

---


## English

| 1. **Systemrequirement**<br/>2. **To explain the files**<br/>3. **Download**                  |                                    |
|:--------------------------------------------------------------------------------------------- | ---------------------------------- |
| The TopTipper addon gives you a display<br>of the table standings in the LMO's betting game.) | ![](/lmo/help/media/toptipper.png) |


---

### Systemrequirement

- Runnable LMO 4 from Beta 3 with betting game

---

### To explain the files

The content of the download consists of 4 files.



**toptipper.php**

Addon File<br>
is in the folder 'addon/tipp/'



**kal.tip**

is in the folder 'config/tipp/'<br>
Is for configuration and can be renamed as desired. The main thing is that the file extension *.tipp remains and the new name is also taken into account when integrating.  

- The content of the file consists of

| [config]          |                                                                                              |
| ----------------- | -------------------------------------------------------------------------------------------- |
| modus=1           | **// You might be able to use the mode at 1 again**                                          |
| anzahl_tipper=10  | **// Number of tipsters in the ad**                                                          |
| all=0             | **// 0 or 1, 0 shows the file (one league), 1 shows the added values ​​(for several leagues)** |
| file=erg_dfb.l98  | **// your league**                                                                           |
| template=standard | **// Template name without the ending (.tpl.php)**                                           |



**standard.tpl.php**

is in the folder 'template/tipp/'<br>
The template can be created arbitrarily. Available placeholders are currently:
| placeholder      | Description                                   |
| ----------------:|:--------------------------------------------- |
| `<!--URLTipp-->` | **The link to the betting game**              |
| `<!--gotoTipp-->`| **The name for the link to the betting game** |
| `<!--URLLMO-->`  | **The Link to the LMO**                       |
| `<!--gotoLMO-->` | **The name for the link to the LMO**          |
| `<!--Platz-->`   | **The placement of the tipsters**             |
| `<!--Name-->`    | **The name of the tipsters**                  |
| `<!--Punkte-->`  | **The tipsters' points**                      |



**tipp.php**

is located directly in the root directory of your LMO.

Used to integrate the entire script (adjust content)

- Example:

```php
<?php
  $multi = "kal";  //In this case, the kal.tip file you customized will be integrated.
  require(dirname(__FILE__) . '/init.php');
  include(PATH_TO_ADDONDIR . "/tipp/toptipper.php");
?>
```

---

### Download

- [Download](https://github.com/henshingly/Toptipper/tags)

---
