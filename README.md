# material-components-vue | mdc-web &#9829; vuejs

[![Build Status](https://travis-ci.org/matsp/material-components-vue.svg?branch=master)](https://travis-ci.org/matsp/material-components-web) 
[![npm version](https://badge.fury.io/js/material-components-vue.svg)](https://badge.fury.io/js/material-components-vue)

Ready to use vue components with the styling and behavior of material design - including material-icons.
Actual no deep foundation implementation.

## component architecture principles

* container components e.g. 'Card' have named slots to fill in other components
* sub-components e.g. 'List' for optional content in other components
* state is outside of components and will be passed in as props - maybe modeled
* components react on state changes with actions
* components CSS classes can be modified by props

## component detail design
* optional id on every component
* just one type as prop e.g. Boolean instead of [Boolean, String]
* v-if on tags if needed e.g. v-if="text" 
* v-bind="$attrs" to inherit parent non prop attributes in sub components & v-on="$listeners" to inherit their listeners


## TODO

### Common
* [x] Refactor components
* [x] Import as vuejs plugin
* [] ESM, CommonJS additional to UMD in Webpack build
* [] MaterialIcons as asset inside css?
* [] Documentation of components and their usage (props, events, ...)
* [] Custom elements?
* [] Extra repository for examples
* [] Externalize components?

## Components

### Ready to use components
* Button
* Checkbox
* Dialog
* Card
* Fab
* FormField
* Icon
* IconToggle
* Drawer --> TemporaryDrawer
* Toolbar --> Fixed & Waterfall
* LayoutGrid
* List
* Textfield

### Missing components
* Drawer
* Toolbar
* GridList
* Snackbar
* RadioButton
* SelectMenu
* Slider
* Switch
* Progress
* Menus
* Tabs
