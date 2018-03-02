# uMatrix Recipes
This repository is a set of uMatrix recipes that I have made and are ready to be imported into
uMatrix.

Recipes are a feature being introduced to [uMatrix](https://github.com/gorhill/uMatrix) as described on the 
releases page:
> uMatrix will offer you the ability to import community-contributed 
ruleset recipes which are relevant to the current page

I am no rule making expert, but my goal with this is to update for every site that I create rules for. It is mostly for personal use so certain sites are configured for logins, and for English versions of domains.

**TLDR**: Add `https://raw.githubusercontent.com/themagicteeth/umatrix-recipes/master/recipes.txt` to your imported ruleset
recipes and use them.

## Requirements
1. Firefox Nightly or Developer Edition 
    * must be able to install unsigned extensions
2. uMatrix Beta

## Installing uMatrix Beta 
Before installing an about:config flag must be set.    
1. Copy this into the URL bar: `about:config?filter=xpinstall.signatures.required`
2. Set it to `false`

Currently recipes are only supported in the beta version of uMatrix which is not on the add-on store yet.    
* [Download the beta version here](https://github.com/gorhill/uMatrix/releases)  

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
## Enable and import recipes
Open the settings and go to the Assets tab. Towards the bottom is where recipe lists are added.
Check the box that says `Import...` and paste in this URL:

`https://raw.githubusercontent.com/themagicteeth/umatrix-recipes/master/recipes.txt`

![Import Recipes](https://github.com/themagicteeth/umatrix-recipes/raw/master/imgs/ImportRecipes.JPG "Importing Recipes")

Then click `Apply changes` followed by `Update now`. This will pull in the recipes to be used with uMatrix.

![Apply and update assets](https://github.com/themagicteeth/umatrix-recipes/raw/master/imgs/ApplyChanges.JPG "Apply and update assets")

## Using a recipe
To use a recipe, simply click the puzzle piece icon on a site that has a recipe. The puzzle piece
will change from grey to blue on sites that have a ruleset. To view the rules click the sitename and then apply
them by clicking the lock icon.

![Applying a recipe](https://github.com/themagicteeth/umatrix-recipes/raw/master/imgs/ApplyingRecipe.JPG "Applying a recipe")


## Resources    
[uMatrix Examples of Useful Rulesets](https://github.com/gorhill/uMatrix/wiki/Examples-of-useful-rulesets)    
[uMatrix Recipes](https://github.com/kristerkari/umatrix-recipes)    
[uMatrix Rules - Domain Level](https://github.com/uMatrix-Rules/uMatrix-Rules-Domain)    
[uMatrix Rules - Site Level](https://github.com/uMatrix-Rules/uMatrix-Rules-Site)    
[Official Recipes for uMatrix](https://github.com/uBlockOrigin/uAssets/blob/master/recipes/recipes_en.txt)    
[Reddit Recipes Thread](https://www.reddit.com/r/uMatrix/comments/7v5zrq/recipes/)    
[uMatrix Issue Discussion about Recipes](https://github.com/gorhill/uMatrix/issues/30)    
