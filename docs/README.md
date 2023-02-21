📢 Use this project, [contribute](https://github.com/{OrganizationName}/{AppName}) to it or open issues to help evolve it using [Store Discussion](https://github.com/vtex-apps/store-discussion).

# Custom Diagramation Template
<!-- DOCS-IGNORE:start -->
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
<!-- DOCS-IGNORE:end -->

## Description

The Custom Diagramation Template is a VTEX IO app that allows you to create a custom diagramation template for your store. This app allows you to change the position of the elements on the screen.


![](https://i.imgur.com/pF3Mymz.gif)

## Configuration 

1. Add the Custom Diagramation Template to your theme's dependencies in the manifest.json, for example:
```json
  "dependencies": {
    "{vendor}.special-diagramation": "0.x"
  }
 ```
 
2. install node modules, go to `react` folder and run `yarn`
 
3. Add the `custom-grid` block to your store-theme, for example:
```json
 {
  "flex-layout.col#sustainable__content": {
    "title": "top products desktop layout",
    "children": [
      "rich-text#sustainable__content--title",
      "rich-text#sustainable__content--text",
      "custom-grid"
    ],
    "props": {
      "blockClass": "sustainable__desktop--layout--container--col",
      "width": "100%"
    }
  },
   "custom-grid": {
    "title": "custom grid",
    "props": {
      "blockClass": "sustainable__desktop--layout--container--col--grid"
    },
    "children": [
      "image#custom__grid--one",
      "image#custom__grid--two",
      "image#custom__grid--three",
      "image#custom__grid--four",
      "image#custom__grid--five"
    ]
  },
 }
   ```
|  Block name     | Description                                     |
| -------------- | ----------------------------------------------- |
| `custom-grid` | ![https://img.shields.io/badge/-Mandatory-red](https://img.shields.io/badge/-Mandatory-red)  This is the top-level block that must be declared in a `store-theme` block to render a custom grid block.   |

## Customization

In order to apply CSS customizations in this and other blocks, follow the instructions given in the recipe on [Using CSS Handles for store customization](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization).

|CSS HANDLES |
| ----------- | 
|` grid__${gridType} `|
|` gridTypeClass `|
|` grid__itemBig `|
|` grid__itemSmall `|

<!-- DOCS-IGNORE:start -->

## Contributors ✨

Heric Olier

Thanks goes to these wonderful people:

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind are welcome!

<!-- DOCS-IGNORE:end -->

---- 

Check out some documentation models that are already live: 
- [Breadcrumb](https://github.com/vtex-apps/breadcrumb)
- [Image](https://vtex.io/docs/components/general/vtex.store-components/image)
- [Condition Layout](https://vtex.io/docs/components/all/vtex.condition-layout@1.1.6/)
- [Add To Cart Button](https://vtex.io/docs/components/content-blocks/vtex.add-to-cart-button@0.9.0/)
- [Store Form](https://vtex.io/docs/components/all/vtex.store-form@0.3.4/)
