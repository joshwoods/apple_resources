

- AppKit
- NSColor
-  getCyan(\_:magenta:yellow:black:alpha:) 

Instance Method

# getCyan(\_:magenta:yellow:black:alpha:)

Returns the color object’s CMYK and opacity values.

macOS

``` source
func getCyan(
    _ cyan: UnsafeMutablePointer?,
    magenta: UnsafeMutablePointer?,
    yellow: UnsafeMutablePointer?,
    black: UnsafeMutablePointer?,
    alpha: UnsafeMutablePointer?
)
```

## Parameters 

`cyan`  

Upon return, contains the cyan component of the color object.

`magenta`  

Upon return, contains the magenta component of the color object.

`yellow`  

Upon return, contains the yellow component of the color object.

`black`  

Upon return, contains the black component of the color object.

`alpha`  

Upon return, contains opacity value of the color object.

## Discussion

If `NULL` is passed in as an argument, the method doesn’t set that value. This method works only with objects representing colors in the deviceCMYK. Sending it to other objects raises an exception.

## See Also

### Related Documentation

var blackComponent: CGFloat

The black component value of the color.

var cyanComponent: CGFloat

The cyan component value of the color.

var yellowComponent: CGFloat

The yellow component value of the color.

var magentaComponent: CGFloat

The magenta component value of the color.

var alphaComponent: CGFloat

The alpha (opacity) component value of the color.

### Retrieving Component Values from Color Objects

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s HSB component and opacity values in the respective arguments.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s RGB component and opacity values in the respective arguments.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the grayscale and alpha values of the color.

var numberOfComponents: Int

The number of components in the color.

func getComponents(UnsafeMutablePointer&lt;CGFloat>)

Returns the components of the color as an array.

