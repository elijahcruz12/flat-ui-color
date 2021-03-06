# Flat UI Colors
![Open Collective sponsors](https://img.shields.io/opencollective/sponsors/ecwebservices1?label=Donators&style=for-the-badge) ![Libraries.io dependency status for latest release, scoped npm package](https://img.shields.io/librariesio/release/npm/@ecwebservices/flat-ui-color-sass?style=for-the-badge) ![npm (scoped)](https://img.shields.io/npm/v/@ecwebservices/flat-ui-color-sass?style=for-the-badge)


This package allows you to use the flat ui colors from https://flatuicolors.com/ in sass, with a css file included as well.

## Install
`npm install @ecwebservices/flat-ui-color-sass`

## Usage
You can use this package as a SCSS file, or use the pre-compiled CSS file.

### SCSS

#### Import into webpack or other build systems

You can import it into your webpack, laravel mix, etc. project by using the following line:
`@import "~@ecwebservices/flat-ui-color-sass/scss/flat-ui-colors"`

If your using another pallete (eg. American pallete), just add it's name to it: 

`@import "~@ecwebservices/flat-ui-color-sass/scss/flat-ui-colors-american"`

This will add the scss file to your project. You can also move it from these files into your scss folder as well.

### CSS

You can use the precompiled css by moving it from the `css` to your own asset folders. The compressed and the development versions are named the exact same, but in their own files with maps included. They are seperated by `dev` and `prod` folders.


## Features

There are 2 main ways to features to this package, one is the pre made text and background color classes, the other is the ability to use its variables. 

### Variables

Flat UI Colors Sass has a variable for each color, that you can use exactly how you'd expect in Sass:

`````
   .btn-wet-asphalt {
        background-color: $wet-asphalt;
        color: $clouds;
    }
`````

We have also included a map `$colors` for the colors, to allow you to use the map to create elements for each color at the same time:

````
    @each $name, $color in $colors {
      .btn-#{$name} {
        background-color: $color;
      }
    }
````

## Pre made classes

Inside our SCSS file, we have included two classes for each color, one to change text colors and the other for background colors. You can use them just by using their classes as `.text-* `  and `bg-*`, with the `*` being a color such as: `.text-belize-hole`


## Colors

Please note this list is for the default color palette. To get the colors for any other version, check out the flat ui colors to get the names (eg. pico-8 pink (`pico-8-pink`)) for any other pallete that is already created.

1.  Turquoise: `turquoise`
2.  Green Sea: `green-sea`
3.  Emerald: `emerald`
4.  Nephritis: `nephritis`
5.  Peter River: `peter-river`
6.  Belize Hole: `belize-hole`
7.  Amethyst: `amethyst`
8.  Wisteria: `wisteria`
9.  Wet Asphalt: `wet-asphalt`
10.  Midnight Blue: `mightnight-blue`
11. Sun Flower: `sun-flower`
12. Orange: `orange`
13. Carrot: `carrot`
14. Pumpkin: `pumpkin`
15. Alizarin: `alizarin` 
16. Pomegranite: `pomegranite`
17. Clouds: `clouds`
18. Silver: `silver`
19. Concrete: `concrete`
20. Asbestos: `asbestos`

# Available Palletes

There are currently **2** available palletes:

- Original
- American

# To Come
We have plans to add things like more Flat UI Color Pallettes, such as the British Pallette, American Pallette, and more. We also have plans to add a LESS version, and possibly have other CSS Preprocessors in one package.