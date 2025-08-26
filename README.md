
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
For input defiend
```
sass --no-source-map --watch E:\scss-test
```
    
For global with sub dir (Input & Output Defined):
```
sass --no-source-map --watch E:\xampp\htdocs\blunor\wp-content\plugins\blunor-addons\widgets:E:\xampp\htdocs\blunor\wp-content\plugins\blunor-addons\widgets
```

For same dir:
```
sass --no-source-map --watch .:.
```
