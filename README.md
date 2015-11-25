# kcstar-google-map
A wrapper for GoogleWebComponents/google-map that handles themeing and a couple additional setups for The Kansas City Star.

For the most part, relative variables are passed through to the child google-map component. Having said that, this component
does not pass through every variable. Check the source code to see which ones are available.

## Themes

One of the primary goals of this component is to store and provide a delivery method for styling themes created by the art
department. The `urban-theme` component is included by default. Others are available and must be included manaully into each
project. New themes can be created as well for a specific project. 

When the theme property is changed, Polymer will create an element using the string of the theme property. If there is a
styles property for that element, that property will replace the map styles.

## Disable Panning

On occasion we want to provide an image-like experience more than an interactive map. To disable the ability to pan/drag the
map, set the `disable-pan` attribute.

## Enable The UI

The UI elements are disabled by default and can be toggled on using the `enable-ui` attribute.
