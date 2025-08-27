
## My default VSCode setting with live-sass compiler
``` json
"liveSassCompile.settings.formats": [

    {
        "format": "expanded",
        "extensionName": ".css",
        "savePath": null,
        "savePathReplacementPairs": null
    }
],
"explorer.confirmDelete": false,
"liveSassCompile.settings.generateMap": false,
"liveSassCompile.settings.autoprefix": [

],
"liveSassCompile.settings.forceBaseDirectory": "",
"workbench.panel.defaultLocation": "right",
"editor.cursorBlinking": "expand",
"security.workspace.trust.untrustedFiles": "open",
```

## Compile SASS with cmd

Install SASS:
```
npm install -g sass
```
For all dir with sub dir:
```
sass --no-source-map --watch .:.
```
For this directory only:
```
sass --no-source-map --watch "./":"./"
```
For selected file:
```
sass --no-source-map --watch style.scss:style.css main.scss:main.css
```
Each .scss → its own .css in scss/ :
```
sass --no-source-map "./":"./scss/"
```
All SCSS into a single CSS
```
sass --no-source-map ./:"./scss/style.css"
```
