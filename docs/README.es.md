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
  Entorno de escritorio totalmente personalizable para Windows
  <br/>
  Disponible en más de 70 idiomas
</h2>

<div align="center"> 

[![Colaboradores](https://img.shields.io/github/contributors/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/graphs/contributors)
[![Última modificación](https://img.shields.io/github/last-commit/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/commits/main)
[![Versión](https://img.shields.io/github/v/release/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/releases)
[![Descargas](https://img.shields.io/github/downloads/eythaann/seelen-ui/total.svg)](https://github.com/eythaann/seelen-ui/releases)

</div>

<img src="./documentation/images/preview.png" width="100%" alt="Captura de pantalla de Seelen UI mostrando un entorno de escritorio personalizado">

<table align="center">
  <tr>
    <td align="center">
      <a
        href="https://apps.microsoft.com/detail/Seelen%20UI/9p67c2d4t9fb?mode=full"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Descargar Seelen UI desde la Microsoft Store">
        <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="250px" alt="Descargar Seelen UI desde la Microsoft Store">
      </a>
    </td>
    <td align="center">
      <a
        href="https://discord.gg/ABfASx5ZAJ"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Únete a la comunidad de Seelen UI en Discord">
        <img src="./documentation/images/discord.png" width="230px" alt="Únete a la comunidad de Seelen UI en Discord">
      </a>
    </td>
  </tr>
</table>

## Tabla de contenidos
- [Descripción general](#descripción-general)
- [Instalación](#instalación)
  - [Microsoft Store (recomendada)](#microsoft-store-emrecomendadaem)
  - [Winget](#winget)
  - [Instalador .msix](#instalador-msix)
  - [Instalador .exe](#instalador-exe)
- [Uso](#uso)
- [Próximas funciones](#próximas-funciones)
- [Documentación](#documentación)
  - [Idiomas](./documentation/languages.md)
  - [Barra de herramientas](./documentation/toolbar.md)
  - [Temas](./documentation/themes.md)
  - [Administrador de ventanas](./documentation/window_manager.md)
  - [Proyecto](./documentation/project.md)
- [Contribuciones](#contribuciones)
- [Licencia](#licencia)
- [Contacto](#contacto)

## Descripción general
Seelen UI es una herramienta diseñada para mejorar la experiencia de escritorio en Windows, centrándose en la personalización y la productividad. Se integra sin problemas en su sistema, ofreciendo una variedad de funciones que le permiten personalizar su escritorio y optimizar su flujo de trabajo.

* **Personalice su escritorio**: Seelen UI le permite adaptar su escritorio a su estilo y necesidades. Puede ajustar menús, widgets y otros elementos para crear un espacio de trabajo a su medida.

  ![Seelen UI Escritorio Minimalista](./documentation/images/preview2.png)

<br/>

* **Mejore su productividad**: Seelen UI le ayuda a organizar su escritorio de forma eficiente. Con un Administrador de Ventanas en mosaico, las ventanas se organizan automáticamente para facilitar la multitarea, haciendo que su trabajo sea más fluido.

  ![Seelen UI Administrador de Ventanas en mosaico](./documentation/images/twm_preview.png)

<br/>

* **Disfrute de su música**: Con un módulo de medios integrado compatible con la mayoría de los reproductores, Seelen UI le permite disfrutar de su música sin interrupciones. Puede pausar, reanudar y saltar canciones sin necesidad de abrir ventanas adicionales.

  ![Seelen UI Módulo de Medios](./documentation/images/media_module_preview.png)

<br/>

* **Sea más rápido**: Con un lanzador de aplicaciones inspirado en Rofi, Seelen UI ofrece una forma simple e intuitiva de acceder rápidamente a sus aplicaciones y ejecutar comandos.

  ![Seelen UI Lanzador de Aplicaciones](./documentation/images/app_launcher_preview.png)

<br/>

* **Configuración amigable para el usuario**: Seelen UI ofrece una interfaz intuitiva para facilitar la personalización. Ajuste configuraciones como temas, diseños de la barra de tareas, iconos, etc., con unos pocos clics.

  ![Seelen UI Configuración](./documentation/images/settings_preview.png)

<br/>

## Instalación
> **⚠️ Advertencia**: Seelen UI requiere que el runtime de WebView esté instalado. En Windows 11, viene preinstalado con el sistema. Sin embargo, en Windows 10, el runtime de WebView se incluye con el instalador `setup.exe`. Además, Microsoft Edge es necesario para que la aplicación funcione correctamente. Algunos usuarios pueden haber modificado su sistema y eliminado Edge, por lo que asegúrese de que tanto Edge como el runtime de WebView estén instalados en su sistema.

> **🗒️ Nota**: En instalaciones recientes de Windows, la aplicación puede mostrar una pantalla blanca o negra. Solo necesita actualizar su Windows a través de Windows Update y reiniciar su PC.

Puede elegir entre diferentes opciones de instalación según sus preferencias:

### Microsoft Store <em>(recomendada)</em>
Descargue la última versión desde la página de la [Tienda](https://www.microsoft.com/store/productId/9P67C2D4T9FB?ocid=pdpshare). Esta es la opción recomendada porque recibirá actualizaciones y una versión segura del programa.

***Nota***: Puede tardar entre 1 y 3 días hábiles en reflejarse los cambios en la Microsoft Store, ya que las actualizaciones son aprobadas manualmente.

### Winget
Instale la última versión utilizando:

``` pwsh
winget install --id Seelen.SeelenUI
``` 
> Esta opción también utiliza el paquete firmado `.msix` y garantiza que tenga la última versión segura. Al igual que en Microsoft Store, puede tardar entre 1 y 3 días hábiles para que los cambios se reflejen en Winget, ya que las actualizaciones son aprobadas manualmente por personas en el proyecto `winget-pkg`.

### Instalador .msix
Descargue el instalador `.msix` desde la página de [Releases](https://github.com/eythaann/seelen-ui/releases). Este paquete está firmado, asegurando una instalación segura. Esta es la misma opción que la de la Microsoft Store, pero es un instalador portátil.

### Instalador .exe
Descargue la última versión desde la página de [Releases](https://github.com/eythaann/seelen-ui/releases) y ejecute el instalador `setup.exe`. Esta opción es menos recomendada, ya que el instalador no está firmado, lo que puede hacer que algunos programas antivirus lo marquen como una posible amenaza. El `setup.exe` se actualiza con más rapidez que las versiones de la Microsoft Store o Winget y también recibe notificaciones sobre nuevas versiones.

## Uso

Una vez instalado o extraído, simplemente abra el programa. La interfaz gráfica fácil de usar e intuitiva lo guiará en el proceso de configuración. Personalice su entorno de escritorio sin esfuerzo.

## Documentación

Para obtener detalles más profundos sobre varios aspectos de Seelen UI, explore los siguientes documentos:
- [Idiomas](./documentation/languages.md) - Información sobre las traducciones.
- [Barra de herramientas](./documentation/toolbar.md) - Detalles sobre la personalización y uso de la barra de herramientas.
- [Temas](./documentation/themes.md) - Guía para crear y aplicar temas.
- [Administrador de ventanas](./documentation/windows_manager.md) - Instrucciones sobre la configuración del administrador de ventanas.
- [Proyecto](./documentation/project.md) - Información general sobre el proyecto y su estructura.

## Próximas funciones

¡Estoy emocionado de compartir algunas de las próximas características de Seelen UI! Aquí tiene un adelanto de lo que está planeado para el futuro:

### ~~Lanzador de aplicaciones~~ ✅
Estoy planeando desarrollar un lanzador de aplicaciones inspirado en [Rofi](https://github.com/davatorium/rofi) en Linux. Esta función proporcionará una forma elegante y altamente personalizable de acceder rápidamente a sus aplicaciones.

![Vista previa del lanzador de aplicaciones](https://raw.githubusercontent.com/adi1090x/files/master/rofi/previews/colorful/main.gif)
*Imagen cortesía de [rofi-themes](https://github.com/dctxmei/rofi-themes)*

### Widgets emergentes personalizables
Planeo introducir un conjunto de widgets emergentes totalmente personalizables, similares a las funciones disponibles en [EWW](https://github.com/elkowar/eww). Estos widgets serán altamente configurables y adaptables a sus necesidades, proporcionando una forma mejorada e interactiva de gestionar su entorno de escritorio.

![Vista previa de los widgets personalizables](https://raw.githubusercontent.com/adi1090x/widgets/main/previews/dashboard.png)
*Imagen cortesía de [adi1090x](https://github.com/adi1090x/widgets)*

### Personalización de Alt + Tab (cambio de tareas)
Un sistema Alt + Tab mejorado para el cambio de tareas está en proceso. Esto ofrecerá una experiencia más visual y funcional, permitiendo transiciones más suaves entre aplicaciones y ventanas abiertas.

### Visualizador de escritorios virtuales y animaciones personalizables
También estoy trabajando en un visualizador de escritorios virtuales personalizados y en animaciones dinámicas para mejorar la navegación entre los diferentes espacios de trabajo. Esto proporcionará una experiencia multitarea más intuitiva e inmersiva.

¡Esté atento a más actualizaciones mientras desarrollo estas funciones! Aprecio su apoyo y entusiasmo.

¡Feliz personalización!

El equipo de Seelen UI

## Contribuciones

¡Agradecemos las contribuciones!
* Lea las [Directrices de Contribución](CONTRIBUTING) para comenzar con los términos.
* Lea la [Documentación del Proyecto](documentation/project.md) para comprender la estructura del proyecto y cómo usarlo.

## Licencia

Consulte el archivo [LICENSE](LICENSE) para obtener detalles.

## Contacto

Para consultas y soporte, contácteme en [Discord](https://discord.gg/ABfASx5ZAJ).

## ¡Hasta luego!
