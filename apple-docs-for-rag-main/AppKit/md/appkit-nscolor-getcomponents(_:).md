

- AppKit
- NSColor
-  getComponents(\_:) 

Instance Method

# getComponents(\_:)

Returns the components of the color as an array.

macOS

``` source
func getComponents(_ components: UnsafeMutablePointer)
```

## Parameters 

`components`  

An array containing the components of the color object as `float` values.

## Discussion

You can invoke this method on `NSColor` objects created from custom color spaces to get the individual floating-point components, including alpha. Raises an exception if the receiver doesn’t have floating-point components. To find out how many components are in the `components` array, use the numberOfComponents property.

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

var numberOfComponents: Int

The number of components in the color.

