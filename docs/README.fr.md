<h1 align="center">
  <img src="documentation/images/logo.svg" width="44" align="top" alt="Logo de Seelen UI" />
  Seelen UI
</h1>

- [English](/README.md)
- [中文](/docs/README.zh.md)
- [Français](/docs/README.fr.md)
- [Español](/docs/README.es.md)
- [Deutsch](/docs/README.de.md)

<h2 align="center">
  Environnement de bureau entièrement personnalisable pour Windows
  <br/>
  Disponible en plus de 70 langues
</h2>

<div align="center"> 

[![Contributeurs](https://img.shields.io/github/contributors/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/graphs/contributors)
[![Dernier Commit](https://img.shields.io/github/last-commit/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/commits/main)
[![Version](https://img.shields.io/github/v/release/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/releases)
[![Téléchargements](https://img.shields.io/github/downloads/eythaann/seelen-ui/total.svg)](https://github.com/eythaann/seelen-ui/releases)

</div>

<img src="./documentation/images/preview.png" width="100%" alt="Capture d'écran du bureau Seelen UI montrant un environnement de bureau personnalisé">

<table align="center">
  <tr>
    <td align="center">
      <a
        href="https://apps.microsoft.com/detail/Seelen%20UI/9p67c2d4t9fb?mode=full"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Télécharger Seelen UI depuis le Microsoft Store">
        <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="250px" alt="Télécharger Seelen UI depuis le Microsoft Store">
      </a>
    </td>
    <td align="center">
      <a
        href="https://discord.gg/ABfASx5ZAJ"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Rejoindre la communauté Seelen UI sur Discord">
        <img src="./documentation/images/discord.png" width="230px" alt="Rejoindre la communauté Seelen UI sur Discord">
      </a>
    </td>
  </tr>
</table>

## Table des matières
- [Aperçu](#aperçu)
- [Installation](#installation)
  - [Microsoft Store (recommandé)](#microsoft-store-recommandé)
  - [Winget](#winget)
  - [Programme d'installation .msix](#programme-dinstallation-msix)
  - [Programme d'installation .exe](#programme-dinstallation-exe)
- [Utilisation](#utilisation)
- [Fonctionnalités à venir](#fonctionnalités-à-venir)
- [Documentation](#documentation)
  - [Langues](./documentation/languages.md)
  - [Barre d'outils](./documentation/toolbar.md)
  - [Thèmes](./documentation/themes.md)
  - [Gestionnaire de fenêtres](./documentation/window_manager.md)
  - [Projet](./documentation/project.md)
- [Contributions](#contributions)
- [Licence](#licence)
- [Contact](#contact)

## Aperçu
Seelen UI est un outil conçu pour améliorer l'expérience de bureau Windows en se concentrant sur la personnalisation et la productivité. Il s'intègre facilement à votre système, offrant une gamme de fonctionnalités qui vous permettent de personnaliser votre bureau et d'optimiser votre flux de travail.

* **Personnalisez votre bureau** : Seelen UI vous permet de configurer votre bureau selon vos préférences. Vous pouvez ajuster les menus, les widgets et d'autres éléments pour créer un espace de travail optimal.

  ![Seelen UI Bureau Minimaliste](./documentation/images/preview2.png)

<br/>

* **Améliorez votre productivité** : Seelen UI vous aide à organiser efficacement votre bureau. Avec un gestionnaire de fenêtres à tuiles, les fenêtres se disposent automatiquement pour favoriser le multitâche, rendant votre travail plus fluide.
  
  ![Gestionnaire de fenêtres à tuiles Seelen UI](./documentation/images/twm_preview.png)

<br/>

* **Profitez de votre musique** : Avec un module multimédia intégré compatible avec la plupart des lecteurs de musique, Seelen UI vous permet de profiter de votre musique sans interruption. Vous pouvez mettre en pause, reprendre et changer de piste à tout moment sans ouvrir d'autres fenêtres.
  
  ![Module multimédia Seelen UI](./documentation/images/media_module_preview.png)

<br/>

* **Soyez plus rapide !** : Avec un lanceur d'applications inspiré de Rofi, Seelen UI offre une façon simple et intuitive d'accéder rapidement à vos applications et d'exécuter des commandes.

  ![Lanceur d'applications Seelen UI](./documentation/images/app_launcher_preview.png)

<br/>

* **Configuration conviviale** : Seelen UI propose une interface intuitive pour personnaliser facilement les paramètres comme les thèmes, la disposition de la barre des tâches, les icônes, etc. En quelques clics seulement.

  ![Paramètres Seelen UI](./documentation/images/settings_preview.png)

<br/>

## Installation
> **⚠️ Avertissement** : Seelen UI nécessite l'installation de WebView. Sur Windows 11, il est préinstallé, mais sur Windows 10, WebView est inclus dans l'installateur `setup.exe`. De plus, Microsoft Edge est nécessaire pour un fonctionnement correct. Veuillez vérifier que Edge et WebView sont installés sur votre système.

> **🗒️ Remarque** : Sur une nouvelle installation de Windows, l'application peut afficher un écran blanc ou noir. Vous devez mettre à jour Windows via Windows Update, puis redémarrer votre PC.

Vous avez le choix entre plusieurs options d'installation en fonction de vos préférences：

### Microsoft Store <em>(recommandé)</em>
Téléchargez la dernière version depuis la [page du Microsoft Store](https://www.microsoft.com/store/productId/9P67C2D4T9FB?ocid=pdpshare). Cette option est recommandée, car vous recevrez les mises à jour et une version sécurisée du programme. 

***Remarque*** : Les changements peuvent prendre environ 1 à 3 jours ouvrables pour apparaître sur le Microsoft Store, car les mises à jour sont validées manuellement.

### Winget
Installez la dernière version avec la commande suivante：

``` pwsh 
winget install --id Seelen.SeelenUI
```
Cette option utilise également le package signé `.msix` et garantit que vous disposez de la dernière version sécurisée. Comme pour le Microsoft Store, les changements peuvent prendre 1 à 3 jours ouvrables pour être reflétés dans Winget.

### Programme d'installation .msix
Téléchargez le fichier `.msix` depuis la [page des versions](https://github.com/eythaann/seelen-ui/releases). Ce package est signé, garantissant une installation sécurisée. C'est la même option que le Microsoft Store, mais en version portable.

### Programme d'installation .exe
Téléchargez la dernière version depuis la [page des versions](https://github.com/eythaann/seelen-ui/releases) et exécutez le programme `setup.exe`. Cette option est moins recommandée car l'installateur n'est pas signé, ce qui pourrait entraîner des avertissements de certains antivirus. Le `setup.exe` est mis à jour plus rapidement que les versions du Microsoft Store ou de Winget.

## Utilisation

Une fois installé ou extrait, ouvrez simplement le programme. L'interface intuitive vous guidera à travers le processus de configuration. Personnalisez votre environnement de bureau en toute simplicité.

## Documentation

Pour des détails approfondis sur différents aspects de Seelen UI, explorez les documents suivants :
- [Langues](./documentation/languages.md) - Informations sur les traductions.
- [Barre d'outils](./documentation/toolbar.md) - Détails sur la personnalisation et l'utilisation de la barre d'outils.
- [Thèmes](./documentation/themes.md) - Instructions pour créer et appliquer des thèmes.
- [Gestionnaire de fenêtres](./documentation/window_manager.md) - Instructions sur la configuration du gestionnaire de fenêtres.
- [Projet](./documentation/project.md) - Informations générales sur le projet et sa structure.

## Fonctionnalités à venir

Je suis heureux de partager les fonctionnalités à venir de Seelen UI ! Voici un aperçu des projets en cours：

### ~~Lanceur d'applications~~ ✅
Je prévois de développer un lanceur d'applications inspiré par [Rofi](https://github.com/davatorium/rofi) sous Linux. Cette fonctionnalité offrira un moyen élégant et hautement personnalisable d'accéder rapidement à vos applications.

![Aperçu du lanceur d'applications](https://raw.githubusercontent.com/adi1090x/files/master/rofi/previews/colorful/main.gif)
*Image avec l'aimable autorisation de [rofi-themes](https://github.com/dctxmei/rofi-themes)*

### Widgets contextuels personnalisables
Je vise à introduire un ensemble de widgets contextuels personnalisables, similaires aux fonctionnalités de [EWW](https://github.com/elkowar/eww). Ces widgets seront hautement configurables et adaptés à vos besoins, offrant un moyen interactif et amélioré de gérer votre bureau.

![Aperçu des widgets personnalisables](https://raw.githubusercontent.com/adi1090x/widgets/main/previews/dashboard.png)
*Image avec l'aimable autorisation de [adi1090x](https://github.com/adi1090x/widgets)*

### Système de changement de tâche Alt + Tab personnalisé
Un système Alt + Tab amélioré pour le changement de tâches est en préparation. Cela offrira une expérience visuelle et fonctionnelle améliorée, permettant des transitions plus fluides entre les applications et fenêtres ouvertes.

### Visualiseur de bureaux virtuels et animations
Je travaille également sur un visualiseur de bureaux virtuels personnalisé et des animations dynamiques pour faciliter la navigation entre les espaces de travail. Cela apportera une expérience de multitâche plus intuitive et immersive.

Restez à l'écoute pour plus de mises à jour ! Votre soutien et enthousiasme sont appréciés！

L’équipe Seelen UI

## Contributions

Les contributions sont les bienvenues !
* Lisez le [Guide de contribution](CONTRIBUTING) pour vous familiariser avec les conditions.
* Consultez la [Documentation du projet](documentation/project.md) pour comprendre la structure du projet et son utilisation.

## Licence

Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## Contact

Pour toute question ou support, veuillez me contacter sur [Discord](https://discord.gg/ABfASx5ZAJ).

## À bientôt

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
