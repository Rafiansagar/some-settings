
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
    open cmd
    npm install -g sass
    sass --no-source-map --watch E:\scss-test
    or this for all sub directorys
    sass --no-source-map --watch E:\xampp\htdocs\blunor\wp-content\plugins\blunor-addons\widgets:E:\xampp\htdocs\blunor\wp-content\plugins\blunor-addons\widgets
