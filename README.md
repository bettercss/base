# Base

The `Base` module contains tools, normalization and resets for the BetterCSS toolkit.  

## Installation

Install via [npm](http://npmjs.org/): 
 
 	npm install bettercss-base
    
## Configuration Variables

```scss
// Base spacing unit defaults to 18px 
$bc-b-spacing-unit 

// Base font-size defaults to 14px
$bc-b-font-size 

// Base line-height defaults to 18px
$bc-b-line-height 

// Array of heading sizes from h1-h6
$bc-b-headings

// Array of z-index layers 
$bc-b-z-index-layers 

// Array of breakpoints
$bc-b-responsive-breakpoints 

// Base link color defaults to #000
$bc-b-links-color-text

// Base font-family defaults to 'Helvetica Neue', Helvetica, Arial sans-serif
$bc-b-page-font-family 

// Base background color defaults to #fff
$bc-b-page-color-background

// Base text color defaults to #333
$bc-b-page-color-text
```

## Available Tools
 
### Functions
 
 ```scss
 // Convert any px value into its rem equivalent.
 bc-rem($number);
 ```
 
### Mixins

 ```scss
// Generates dimension classes.
@bc-dimensions($columns, $breakpoint: null, $selector-prefix: 'u-'); 

// Generates a font-size and a corresponding line-height that sits on the baseline grid.
@bc-font-size($font-size, $line-height: auto, $important: false);

// Create a declaration whose value is a rem unit. Also provide pixel fallback.
@bc-rem($peroperty, $value); 

// Micro clearfix hack
@bc-clearfix($important: false);
 
// Simple truncation mixin to cut off text using an ellipsis after a certain width.
@bc-truncate($width: 100%);

// Creates isosceles triangles.
@bc-css-triangle($triangle-size, $triangle-color, $triangle-direction);

// Implements media queries for selectors.
@bc-media-query($breakpoint-name);

// Generate Responsive Classes
@bc-generate-responsive-classes();

// Implements z-index layer for selectors.
@bc-z-index($layer, $important: false);

// Generate Z-index Classes
@bc-generate-z-index-classes();
```