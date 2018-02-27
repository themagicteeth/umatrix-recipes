# umatrix-recipes
Recipes for uMatrix    

## These rules expect uMatrix to be configured globally the following way:
### Matrix
![uMatrix Global Configuration](https://github.com/themagicteeth/umatrix-recipes/raw/master/imgs/uMatrixGloablConfig.JPG "uMatrix Global Configuration")
 
 This translates to the following rules:
  
    * * * block
    * 1st-party css allow
    * 1st-party image allow

### Switches
![uMatrix Global Switches](https://github.com/themagicteeth/umatrix-recipes/raw/master/imgs/uMatrixGloablSwitches.JPG "uMatrix Global Switches")

This translates to the following rules:

    https-strict: * true
    no-workers: * true
    noscript-spoof: * true
    referrer-spoof: * true

## Resources    
[uMatrix Examples of Useful Rulesets](https://github.com/gorhill/uMatrix/wiki/Examples-of-useful-rulesets)    
[uMatrix Recipes](https://github.com/kristerkari/umatrix-recipes)    
[uMatrix Rules - Domain Level](https://github.com/uMatrix-Rules/uMatrix-Rules-Domain)    
[uMatrix Rules - Site Level](https://github.com/uMatrix-Rules/uMatrix-Rules-Site)    
[Official Recipes for uMatrix](https://github.com/uBlockOrigin/uAssets/blob/master/recipes/recipes_en.txt)    
[Reddit Recipes Thread](https://www.reddit.com/r/uMatrix/comments/7v5zrq/recipes/)    