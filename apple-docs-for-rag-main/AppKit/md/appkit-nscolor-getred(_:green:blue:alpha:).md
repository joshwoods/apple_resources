

- AppKit
- NSColor
-  getRed(\_:green:blue:alpha:) 

Instance Method

# getRed(\_:green:blue:alpha:)

Returns the color object’s RGB component and opacity values in the respective arguments.

macOS

``` source
func getRed(
    _ red: UnsafeMutablePointer?,
    green: UnsafeMutablePointer?,
    blue: UnsafeMutablePointer?,
    alpha: UnsafeMutablePointer?
)
```

## Parameters 

`red`  

Upon return, contains the red component of the color object.

`green`  

Upon return, contains the green component of the color object.

`blue`  

Upon return, contains the blue component of the color object.

`alpha`  

Upon return, contains the opacity value of the color object.

## Discussion

If `NULL` is passed in as an argument, the method doesn’t set that value. This method works only with objects representing colors in the calibratedRGB or deviceRGB color space. Sending it to other objects raises an exception.

## See Also

### Related Documentation

var blueComponent: CGFloat

The blue component value of the color.

var redComponent: CGFloat

The red component value of the color.

var alphaComponent: CGFloat

The alpha (opacity) component value of the color.

var greenComponent: CGFloat

The green component value of the color.

### Retrieving Component Values from Color Objects

func getCyan(UnsafeMutablePointer&lt;CGFloat>?, magenta: UnsafeMutablePointer&lt;CGFloat>?, yellow: UnsafeMutablePointer&lt;CGFloat>?, black: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s CMYK and opacity values.

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s HSB component and opacity values in the respective arguments.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the grayscale and alpha values of the color.

var numberOfComponents: Int

The number of components in the color.

func getComponents(UnsafeMutablePointer&lt;CGFloat>)

Returns the components of the color as an array.

