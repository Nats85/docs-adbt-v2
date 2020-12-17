---
title: Despliegue de base de datos
chapter: "problemas"
---

## Error al desplegar o actualizar una versión de la base de datos

<span style="color: red;">
System.ComponentModel.Win32Exception (0x80004005): The system cannot find the file specified
</span>

![]({{ site.baseurl }}/assets/images/update_package_error.png)

Si al momento de actualizar una base de datos el sistema arroja un error de **Win32Exception** con codigo **0x80004005**, es posible que haga falta instalar el **SQLCommandLine** en la maquina. Dirijase a la sección [Requisitos de instalacion](/adbt/pages/requisitos/01-Requisitos para la instalación.html) e instale los programas necesarios. Para finalizar reinicie Aranda DB Tools.

## Fallo al ejecutar el script

<span style="color: red;">
Aranda.ADBT.Exceptions.DatabaseToolsException: ScriptFail
</span>

![]({{ site.baseurl }}/assets/images/script_failed.png)

Si ocurren errores durante la ejecución y arroja el sistema la excepción anterior, antes de continuar verifique que la estructura de la base de datos coincida con al versión que va actualizar.

## Paquetes faltantes

<span style="color: red;">
Aranda.ADBT.Exceptions.DatabaseToolsException: InvalidUpdate
</span>

![]({{ site.baseurl }}/assets/images/packages_notfound.png)

Si va actualizar la base de datos (Ejemplo: De 9.5.0 a 9.5.6) tenga en cuenta que se necesitan las versiones intermedias, verifique que existan las demas versiones en la carpeta, si no existen, dirijase a la sección de [Packages](/adbt/pages/modulos/01-Packages (paquetes).html) y siga los pasos.

## Paquete no encontrado

<span style="color: red;">
Aranda.ADBT.Exceptions.DatabaseToolsException: PackageNotFound ---> System.IO.FileNotFoundException: Could not find file '...\Packages\SqlServer\9.X.X.zip'.
</span>

![]({{ site.baseurl }}/assets/images/package_notfound.png)

Verifique que en el Tab de **Packages** los paquetes tengan el estado **Ok**, si no es así, dirijase a la sección [Packages](/adbt/pages/modulos/01-Packages (paquetes).html).


