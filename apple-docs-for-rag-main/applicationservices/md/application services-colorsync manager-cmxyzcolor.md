

- Application Services
- ColorSync Manager
-  CMXYZColor 

Structure

# CMXYZColor

Contains values for a color specified in XYZ color space.

macOS 10.0+

``` source
struct CMXYZColor
```

## Overview

Three color component values defined by the `CMXYZComponent` type definition combine to form a color value specified in the XYZ color space. The color value is defined by the `CMXYZColor` type definition.

Your application uses the `CMXYZColor` data structure to specify a color value in the `CMColor` union to use in general purpose color matching, color checking, or color conversion. You also use the `CMXYZColor` data structure to specify the XYZ white point reference used in the conversion of colors to or from the XYZ color space.

## Topics

### Initializers

init()

init(X: CMXYZComponent, Y: CMXYZComponent, Z: CMXYZComponent)

### Instance Properties

var X: CMXYZComponent

var Y: CMXYZComponent

var Z: CMXYZComponent

