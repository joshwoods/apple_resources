

- AppKit
- NSColor
-  getHue(\_:saturation:brightness:alpha:) 

Instance Method

# getHue(\_:saturation:brightness:alpha:)

Returns the color object’s HSB component and opacity values in the respective arguments.

macOS

``` source
func getHue(
    _ hue: UnsafeMutablePointer?,
    saturation: UnsafeMutablePointer?,
    brightness: UnsafeMutablePointer?,
    alpha: UnsafeMutablePointer?
)
```

## Parameters 

`hue`  

Upon return, contains the hue component of the color object.

`saturation`  

Upon return, contains the saturation component of the color object.

`brightness`  

Upon return, contains the brightness component of the color object.

`alpha`  

Upon return, contains the opacity value of the color object.

## Discussion

If `NULL` is passed in as an argument, the method doesn’t set that value. This method works only with objects representing colors in the calibratedRGB or deviceRGB color space. Sending it to other objects raises an exception.

## See Also

### Related Documentation

var brightnessComponent: CGFloat

The brightness component value of the color.

var hueComponent: CGFloat

The hue component value of the color.

var alphaComponent: CGFloat

The alpha (opacity) component value of the color.

var saturationComponent: CGFloat

The saturation component value of the color.

### Retrieving Component Values from Color Objects

func getCyan(UnsafeMutablePointer&lt;CGFloat>?, magenta: UnsafeMutablePointer&lt;CGFloat>?, yellow: UnsafeMutablePointer&lt;CGFloat>?, black: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s CMYK and opacity values.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s RGB component and opacity values in the respective arguments.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the grayscale and alpha values of the color.

var numberOfComponents: Int

The number of components in the color.

func getComponents(UnsafeMutablePointer&lt;CGFloat>)

Returns the components of the color as an array.

