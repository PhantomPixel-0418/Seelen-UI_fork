<h1 align="center">
  <img src="documentation/images/logo.svg" width="44" align="top" alt="Seelen UI Logo" />
  Seelen UI
</h1>

- [English](/README.md)  
- [中文](/docs/README.zh.md)  
- [Français](/docs/README.fr.md)  
- [Español](/docs/README.es.md)  
- [Deutsch](/docs/README.de.md)  

<h2 align="center">
  Vollständig anpassbare Desktop-Umgebung für Windows
  <br/>
  In über 70 Sprachen verfügbar
</h2>

<div align="center"> 

[![Contributors](https://img.shields.io/github/contributors/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/graphs/contributors)
[![Last Commit](https://img.shields.io/github/last-commit/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/commits/main)
[![Version](https://img.shields.io/github/v/release/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/releases)
[![Downloads](https://img.shields.io/github/downloads/eythaann/seelen-ui/total.svg)](https://github.com/eythaann/seelen-ui/releases)

</div>

<img src="./documentation/images/preview.png" width="100%" alt="Screenshot of Seelen UI desktop showing a customized desktop environment">

<table align="center">
  <tr>
    <td align="center">
      <a
        href="https://apps.microsoft.com/detail/Seelen%20UI/9p67c2d4t9fb?mode=full"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Download Seelen UI from Microsoft Store">
        <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="250px" alt="Download Seelen UI from Microsoft Store">
      </a>
    </td>
    <td align="center">
      <a
        href="https://discord.gg/ABfASx5ZAJ"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Join the Seelen UI Discord community">
        <img src="./documentation/images/discord.png" width="230px" alt="Join the Seelen UI Discord community">
      </a>
    </td>
  </tr>
</table>

## Inhaltsverzeichnis
- [Übersicht](#übersicht)
- [Installation](#installation)
  - [Microsoft Store (empfohlen)](#microsoft-store-emempfohlenem)
  - [Winget](#winget)
  - [.msix Installer](#msix-installer)
  - [.exe Installer](#exe-installer)
- [Benutzung](#benutzung)
- [Bevorstehende Funktionen](#bevorstehende-funktionen)
- [Dokumentation](#dokumentation)
  - [Sprachen](./documentation/languages.md)
  - [Symbolleiste](./documentation/toolbar.md)
  - [Themen](./documentation/themes.md)
  - [Fenstermanager](./documentation/window_manager.md)
  - [Projekt](./documentation/project.md)
- [Mitwirken](#mitwirken)
- [Lizenz](#lizenz)
- [Kontakt](#kontakt)

## Übersicht
Seelen UI ist ein Tool, das das Windows-Desktop-Erlebnis mit einem Schwerpunkt auf Anpassung und Produktivität verbessert. Es integriert sich nahtlos in Ihr System und bietet eine Vielzahl an Funktionen, die es Ihnen ermöglichen, Ihren Desktop anzupassen und Ihren Arbeitsablauf zu optimieren.

* **Passen Sie Ihren Desktop an**: Mit Seelen UI können Sie Ihren Desktop nach Ihren Bedürfnissen gestalten. Menüs, Widgets und andere Elemente lassen sich anpassen, um eine auf Sie zugeschnittene Arbeitsumgebung zu schaffen.

  ![Seelen UI Minimal Desktop](./documentation/images/preview2.png)

<br/>

* **Steigern Sie Ihre Produktivität**: Seelen UI hilft Ihnen, Ihren Desktop effizient zu organisieren. Mit einem Kachel-Fenstermanager werden Fenster automatisch angeordnet, um Multitasking zu unterstützen und die Arbeit zu optimieren.
  
  ![Seelen UI Tiling Window Manager](./documentation/images/twm_preview.png)

<br/>

* **Genießen Sie Ihre Musik**: Mit einem integrierten Medienmodul, das mit den meisten Musik-Playern kompatibel ist, können Sie Ihre Musik nahtlos genießen. Sie können jederzeit pausieren, fortfahren und Titel überspringen, ohne zusätzliche Fenster öffnen zu müssen.
  
  ![Seelen UI Media Module](./documentation/images/media_module_preview.png)

<br/>

* **Seien Sie schneller!**: Mit einem App-Launcher, inspiriert von Rofi, bietet Seelen UI eine einfache und intuitive Möglichkeit, schnell auf Ihre Anwendungen zuzugreifen und Befehle auszuführen.

  ![Seelen UI App Launcher](./documentation/images/app_launcher_preview.png)

<br/>

* **Benutzerfreundliche Konfiguration**: Seelen UI bietet eine intuitive Oberfläche für eine einfache Anpassung. Einstellungen wie Themen, Taskleisten-Layouts, Symbole usw. lassen sich mit nur wenigen Klicks anpassen.

  ![Seelen UI Settings](./documentation/images/settings_preview.png)

<br/>

## Installation
> **⚠️ Warnung**: Seelen UI erfordert die Installation der WebView-Laufzeitumgebung. Auf Windows 11 ist diese bereits vorinstalliert. Auf Windows 10 ist die WebView-Laufzeitumgebung im `setup.exe`-Installer enthalten. Zusätzlich wird Microsoft Edge benötigt. Stellen Sie sicher, dass sowohl Edge als auch die WebView-Laufzeitumgebung auf Ihrem System installiert sind.

> **🗒️ Hinweis**: Bei frischen Windows-Installationen kann die App einen weißen oder dunklen Bildschirm anzeigen. Führen Sie einfach ein Windows-Update durch und starten Sie Ihren PC neu.

Sie können zwischen verschiedenen Installationsmethoden wählen:

### Microsoft Store <em>(empfohlen)</em>
Laden Sie die neueste Version von der [Store-Seite](https://www.microsoft.com/store/productId/9P67C2D4T9FB?ocid=pdpshare) herunter. Dies ist die empfohlene Option, da Sie Updates und eine sichere Version des Programms erhalten.

***Hinweis***: Es kann 1 bis 3 Werktage dauern, bis Änderungen im Microsoft Store angezeigt werden, da Updates manuell überprüft werden.

### Winget
Installieren Sie die neueste Version mit folgendem Befehl:

``` pwsh
winget install --id Seelen.SeelenUI
``` 
Diese Option verwendet ebenfalls das signierte `.msix`-Paket und stellt sicher, dass Sie die neueste sichere Version erhalten. Ähnlich wie im Microsoft Store kann es 1 bis 3 Werktage dauern, bis Änderungen in Winget angezeigt werden, da Updates im `winget-pkg`-Projekt manuell genehmigt werden.

### .msix Installer
Laden Sie den `.msix`-Installer von der [Releases](https://github.com/eythaann/seelen-ui/releases)-Seite herunter. Dieses Paket ist signiert und bietet eine sichere Installation. Dies entspricht der Microsoft Store-Version, jedoch in Form eines tragbaren Installers.

### .exe Installer
Laden Sie die neueste Version von der [Releases](https://github.com/eythaann/seelen-ui/releases)-Seite herunter und führen Sie den `setup.exe`-Installer aus. Diese Option ist weniger empfehlenswert, da der Installer nicht signiert ist und möglicherweise von einigen Antivirenprogrammen als potenzielle Bedrohung markiert wird. Der `setup.exe`-Installer wird schneller aktualisiert als die Microsoft Store- oder Winget-Versionen und bietet auch Update-Benachrichtigungen bei neuen Versionen.

## Benutzung

Nach der Installation oder dem Extrahieren öffnen Sie einfach das Programm. Die benutzerfreundliche und intuitive GUI leitet Sie durch den Konfigurationsprozess. Passen Sie Ihre Desktop-Umgebung mühelos an.

## Dokumentation

Für detaillierte Informationen zu den verschiedenen Aspekten von Seelen UI werfen Sie einen Blick auf die folgenden Dokumente:
- [Sprachen](./documentation/languages.md) - Informationen zu Übersetzungen.
- [Symbolleiste](./documentation/toolbar.md) - Details zur Anpassung und Verwendung der Symbolleiste.
- [Themen](./documentation/themes.md) - Anleitung zum Erstellen und Anwenden von Themen.
- [Fenstermanager](./documentation/windows_manager.md) - Anweisungen zur Konfiguration des Fenstermanagers.
- [Projekt](./documentation/project.md) - Allgemeine Informationen zum Projekt und zur Struktur.

## Bevorstehende Funktionen

Ich freue mich, einige bevorstehende Funktionen für Seelen UI mit Ihnen zu teilen! Hier ein Ausblick auf das, was geplant ist:

### ~~App-Launcher~~ ✅
Ich plane, einen App-Launcher zu entwickeln, der von [Rofi](https://github.com/davatorium/rofi) auf Linux inspiriert ist. Diese Funktion wird eine elegante und hochgradig anpassbare Möglichkeit bieten, schnell auf Ihre Anwendungen zuzugreifen.

![App Launcher Preview](https://raw.githubusercontent.com/adi1090x/files/master/rofi/previews/colorful/main.gif)
*Bildquelle: [rofi-themes](https://github.com/dctxmei/rofi-themes)*

### Anpassbare Popup-Widgets
Ich plane, eine Reihe vollständig anpassbarer Popup-Widgets einzuführen, ähnlich den Funktionen, die in [EWW](https://github.com/elkowar/eww) verfügbar sind. Diese Widgets werden hochgradig konfigurierbar und anpassbar sein und bieten eine verbesserte und interaktive Möglichkeit, Ihre Desktop-Umgebung zu verwalten.

![Anpassbare Widgets Vorschau](https://raw.githubusercontent.com/adi1090x/widgets/main/previews/dashboard.png)
*Bildquelle: [adi1090x](https://github.com/adi1090x/widgets)*

### Benutzerdefiniertes Alt + Tab (Task-Umschaltung)
Ein verbessertes Alt + Tab-System für die Task-Umschaltung ist in Arbeit. Es wird eine visuell ansprechendere und funktionale Erfahrung bieten, die nahtlose Übergänge zwischen geöffneten Anwendungen und Fenstern ermöglicht.

### Benutzerdefinierte virtuelle Desktops-Anzeige und Animationen
Ich arbeite außerdem an einer benutzerdefinierten virtuellen Desktops-Anzeige sowie dynamischen Animationen, um die Navigation zwischen verschiedenen Arbeitsbereichen zu verbessern. Dies wird eine intuitivere und immersivere Multitasking-Erfahrung ermöglichen.

Bleiben Sie gespannt auf weitere Updates, während ich diese Funktionen entwickle. Vielen Dank für Ihre Unterstützung und Begeisterung!

Viel Spaß beim Anpassen!

Das Seelen UI-Team

## Mitwirken

Beiträge sind willkommen!
* Lesen Sie die [Beitragsrichtlinien](CONTRIBUTING), um sich mit den Bedingungen vertraut zu machen.
* Lesen Sie die [Projektdokumentation](documentation/project.md), um die Projektstruktur zu verstehen und zu lernen, wie man sie verwendet.

## Lizenz

Siehe die [LICENSE](LICENSE)-Datei für Details.

## Kontakt

Für Anfragen und Support kontaktieren Sie mich bitte auf [Discord](https://discord.gg/ABfASx5ZAJ).

## Bis später

```
                   .      .&     _,x&"``
                    & .   &'  ;.&&'
              &.  . &.&     .0&&&;&""`
         .    '&  &.&&&  .&&&&&'
       .&         ;&&& &&&&&'
      &&          &&&&&&&&     &&&
     0&    .     &&&&&&&&""
    &&   .0     &&&&&&&
   0&& .&'     &&&&&&
  :&&&&&    . &&&&& 
  0&&&&    & &&&&&
  &&&&'   &&&&&&&               .&&&x&
  &&&&   :&&&&&0.&'        , .&&&&&&&&&&;.
  &&&&.  &&&&&&&&        .&&&&&&&&&&'               .
  0&&&&  &&&&&&&       ,&&&&&&&&&&&&                &
  :&&&&; &&&&&0       ,;&&&&&&&&&&&             ;  .0
   0&&&&&&&&&&0     ,;&&&&&&&&&&&&&             &  &;
    0&&&&&&&&&&0   :',;".&&&&&&".&             && &0
     0&&&&&&&&&0  ',;',&&&&&" ,&'             &&&&0
      0&&&&&&&&&0 ,x&&&&" .&&&              &&&&0
        0&&&&&& .&&&&"'''"&&"&&            &&&&&0
         0&& .&&;``       `&: :&         &&&&&&0
            &"' &&&&&&&&   &"& &"&   &&&&&&&&0
              0&&&&&&&&&&&&&&&&&&&&&&&&&0
                 0&&&&&&&&&&&&&&&&&&&0         Seelen
                      0&&&&&&&&&0
```
