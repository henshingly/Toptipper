[<img src="https://www.vest-sport.de/forum_files/addon_toptipper.svg">](https://www.vest-sport.de/forum)

# Toptipper

[![GitHub release](https://img.shields.io/github/release/henshingly/Toptipper?include_prereleases=&sort=semver&color=blue)](https://github.com/henshingly/Toptipper/releases/)
[![download-badge](https://img.shields.io/github/downloads/henshingly/Toptipper/total.svg?style=flat-square "Download status")](https://github.com/henshingly/Toptipper/releases/latest "Download status")
[![Donate](https://img.shields.io/badge/-Buy%20me%20a%20coffee-brown.svg)](https://paypal.me/LMOforum)

## Deutsch

| 1. **Systemvoraussetzung**<br/>2. **Zur Erklärung der Dateien**<br/>3. **Download** |                                                          |
|:----------------------------------------------------------------------------------- | -------------------------------------------------------- |
| Das Addon TopTipper zeigt eine Minitabelle<br>der Tipper im Tippspiel Deines LMO's. | ![](https://www.vest-sport.de/forum_files/toptipper.png) |

---

### Systemvoraussetzung

- Lauffähiger LMO 4 mit Tippspiel

---

### Zur Erklärung der Dateien

Der Inhalt des Downloads besteht aus 5 Dateien.

**toptipper.php**

Addon Datei
befindet sich im Ordner 'addon/tipp/'

**kal.tip**

befindet sich im Ordner 'config/tipp/'
Ist für die Konfiguration zuständig und kann beliebig umbenannt werden. Hauptsache die Dateiendung ***.tipp** bleibt bestehen und der neue Name wird auch beim einbinden  berücksichtigt (siehe tipp.php).  

- Der Inhalt der Datei besteht aus  

| [config]          |                                                                                      |
| ----------------- | ------------------------------------------------------------------------------------ |
| modus=1           | **// Modus auf 1 lassen kann man vielleicht noch mal gebrauchen**                    |
| anzahl_tipper=10  | **// Anzahl der Tipper in der Anzeige**                                              |
| all=0             | **// 0 oder 1, 0 zeigt das file (eine Liga), 1 die gesamt.aus (bei mehreren Ligen)** |
| file=erg_dfb.l98  | **// eure Liga**                                                                     |
| template=standard | **// Template Name ohne die Endung (.tpl.php)**                                      |

**standard.tpl.php** und **round.tpl.php** (Beispieltemplates)

befinden sich im Ordner 'template/tipp/'

Die Templates können beliebig erstellt werden. Verfügbare Platzhalter sind derzeit:
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
Diese ist eigentlich nur eine Beispieldatei und dient zum Einbinden des ganzen Scriptes (Inhalt anpassen)

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

- [Download](https://github.com/henshingly/Toptipper/releases/)

---

## English

| 1. **Systemrequirement**<br/>2. **To explain the files**<br/>3. **Download**          |                                                          |
|:------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| The TopTipper addon shows a mini table<br>of the tipsters in your LMO's betting game. | ![](https://www.vest-sport.de/forum_files/toptipper.png) |

---

### Systemrequirement

- Runnable LMO 4 with betting game

---

### To explain the files

The content of the download consists of 5 files.

**toptipper.php**

Addon File
is in the folder 'addon/tipp/'

**kal.tip**

located in the 'config/tipp/' folder
Is responsible for the configuration and can be renamed as desired. The main thing is that the file extension ***.tipp** remains and the new name is also taken into account when integrating (see tipp.php).

- The content of the file consists of

| [config]          |                                                                                                |
| ----------------- | ---------------------------------------------------------------------------------------------- |
| modus=1           | **// You might be able to use the mode at 1 again**                                            |
| anzahl_tipper=10  | **// Number of tipsters in the ad**                                                            |
| all=0             | **// 0 or 1, 0 shows the file (one league), 1 shows the added values ​​(for several leagues)** |
| file=erg_dfb.l98  | **// your league**                                                                             |
| template=standard | **// template name without the ending (.tpl.php)**                                             |

**standard.tpl.php** and **round.tpl.php** (Sample templates)

are in the folder 'template/tipp/'


The templates can be created arbitrarily. Available placeholders are currently:
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
This is actually just an example file and is used to integrate the entire script (adjust content)

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

- [Download](https://github.com/henshingly/Toptipper/releases/)

---
