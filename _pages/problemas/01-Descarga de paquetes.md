---
title: Descarga de paquetes
chapter: "problemas"
---

## No es posible descargar los paquetes
<span style="color: red;">
System.Net.WebException: Unable to connect to the remote server
</span>

![]({{ site.baseurl }}/assets/images/download_package_error.png)

Si presenta un error como el anterior.
1. Verifique si puede acceder desde un navegador a la URL donde se encuentran alojados los paquetes ***http://download.arandasoft.com/ADBT/V9***. Si no tiene acceso a internet puede hacer la implementacion de los paquetes manualmente, para eso dirijase a la sección [Packages](/adbt/pages/modulos/01-Packages (paquetes).html).
1. Si necesita acceder por medio de un proxy haga la respectiva configuracion en **Configure** ubicado en el Tab de **Package**
1. Es posible que el host para la descarga de paquetes no sea el correcto. Verifique la sección **RequestConfiguration** que se encuentra en el archivo de configuración **Aranda.ADBT.Windows.Application.exe.config** ubicado en la carpeta raíz de Aranda DB Tools. Compruebe que la URL del host sea ***http://download.arandasoft.com/ADBT/V9***. 




