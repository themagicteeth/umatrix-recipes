# umatrix-recipes
## Requirements
1. Firefox Nightly or Developer Edition 
  * must be able to install unsigned extensions
2. uMatrix Beta

## Setup
Currently recipes are only supported in the beta version of uMatrix which is not on the add-on store yet.    
[Download the beta version here](https://github.com/gorhill/uMatrix/releases)  
    
Before installing an about:config flag must be set.    
[Click here, and set the value to false](about:config?filter=xpinstall.signatures.required)
    
## These rules expect uMatrix to be configured globally the following way:
### Matrix
![uMatrix Global Configuration](https://github.com/themagicteeth/umatrix-recipes/raw/master/imgs/uMatrixGloablConfig.JPG "uMatrix Global Configuration")
 
This translates to the following rules:
```
* * * block
* 1st-party css allow
* 1st-party image allow
```

### Switches
![uMatrix Global Switches](https://github.com/themagicteeth/umatrix-recipes/raw/master/imgs/uMatrixGloablSwitches.JPG "uMatrix Global Switches")

This translates to the following rules:
```
https-strict: * true
no-workers: * true
noscript-spoof: * true
referrer-spoof: * true
```

## Resources    
[uMatrix Examples of Useful Rulesets](https://github.com/gorhill/uMatrix/wiki/Examples-of-useful-rulesets)    
[uMatrix Recipes](https://github.com/kristerkari/umatrix-recipes)    
[uMatrix Rules - Domain Level](https://github.com/uMatrix-Rules/uMatrix-Rules-Domain)    
[uMatrix Rules - Site Level](https://github.com/uMatrix-Rules/uMatrix-Rules-Site)    
[Official Recipes for uMatrix](https://github.com/uBlockOrigin/uAssets/blob/master/recipes/recipes_en.txt)    
[Reddit Recipes Thread](https://www.reddit.com/r/uMatrix/comments/7v5zrq/recipes/)    