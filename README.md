# Análisis Matemático 3
Universidad Argentina De la Empresa

### Instalación de entorno

Obligatorios

  - Instalar LaTex nativo. En windows se tiene Miktex.
  - En la consola de Miktex seleccionar todos los paquetes (ordenar por no instalados) no instalados, e instalarlos.

Opcionales:

  - Instalar un editor de texto del código. Puede ser uno genérico, como Sublime Text 3, o uno específico como TexMaker.
  - Instalar un visualizador de PDF como Acrobat, o si se prefiere PS también está GhostScript que admite ambos.
  - Configurar el entorno de TexMaker si es que se usó el mismo. En Options -> Configure, tenemos que modificar el campo "ghostscript" y colocar la ruta del archivo gswin64.exe o similar que se obtuvo en la instalación, ejemplo: "C:/Program Files/gs/gs9.27/bin/gswin64.exe". En Dvi Viewer, si es que se necesita el DVI, clocar la ruta de la carpeta de instalación de MikTex, y en PS Viewer de querer formato PS, colocar la carpeta del visualizador, Acrobat Reader también es válido (Usar carpeta Reader que está dentro de la carpeta de instalación).


### Instalación

Para generar el documento PDF se debe abrir una consola de comandos en la carpeta donde se encuentra el proyecto. Acto seguido, ejecutar los siguientes comandos:

```
$ pdfLatex apunte.tex
$ bibtex apunte.tex
$ pdfLatex apunte.tex
$ pdfLatex apunte.tex
```

En las diferentes pasadas se van realizando diferentes cambios en el documento, hasta que al ejecutar la última pasada se genera una versión final de dicho documento. Es importante realizarlas todas.