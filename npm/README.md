## This is some copy+paste stuff for npm, webpack and gulp AND nodejs

### node : <br>
```
sudo apt install curl
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install nodejs build-essential

```

### npm : <br>
```
npm install <name of module>      -> local installation
npm install -g <name of module>   -> global instalation
npm list
npm uninstall -g
npm uninstall
npm -v                            -> version

npm update -g <name of module>    -> update globally

npm install <name of module> --save   ->installation with adding module to dependencies field in package.json file
npm install <name of module> --save-dev ->devDependencies in package.json

npm install   -> installing all modules from package.json

```
<br>

## gulp :

```
npm install --global gulp-cli   -> global installation of CLI tools for gulp 
npm rm --global gulp 

local installation: (needed for every project)

npm init
npm install --save-dev gulp

```
