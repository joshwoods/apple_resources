

- AppKit
- NSColor
-  numberOfComponents 

Instance Property

# numberOfComponents

The number of components in the color.

macOS

``` source
var numberOfComponents: Int { get }
```

## Discussion

This property reflects the number of floating-point component values in the color and includes the alpha component. If the color object does not have any floating-point component values, accessing this property raises an exception.

## See Also

### Related Documentation

var colorSpace: NSColorSpace

The color space associated with the color.

### Retrieving Component Values from Color Objects

func getCyan(UnsafeMutablePointer&lt;CGFloat>?, magenta: UnsafeMutablePointer&lt;CGFloat>?, yellow: UnsafeMutablePointer&lt;CGFloat>?, black: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s CMYK and opacity values.

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s HSB component and opacity values in the respective arguments.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s RGB component and opacity values in the respective arguments.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the grayscale and alpha values of the color.

func getComponents(UnsafeMutablePointer&lt;CGFloat>)

Returns the components of the color as an array.

