
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


## Run cmd on network pc
```
On host pc:
1. Win + I → Apps → Optional Features.
2. Look for OpenSSH Server:
   If not installed → click Add a feature, search “OpenSSH Server”, install it.
3. Start the service:
   Open Services (services.msc), find OpenSSH SSH Server, set Startup Type → Automatic, then Start it.
4. (optional)
   Allow SSH through Firewall:
   # Open Windows Security → Firewall & Network Protection → Allow an app through firewall.
   # Enable OpenSSH Server on private networks.
5. Ensure these lines exist and are not commented
   C:\ProgramData\ssh\sshd_config
   PasswordAuthentication yes
   PubkeyAuthentication yes

On your pc cmd:
ssh userName@192.168.0.138
yes
pass: host pass
```
