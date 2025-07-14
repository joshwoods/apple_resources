

- AppKit
- NSColor
-  getWhite(\_:alpha:) 

Instance Method

# getWhite(\_:alpha:)

Returns the grayscale and alpha values of the color.

macOS

``` source
func getWhite(
    _ white: UnsafeMutablePointer?,
    alpha: UnsafeMutablePointer?
)
```

## Parameters 

`white`  

Upon return, contains the grayscale value of the color object.

`alpha`  

Upon return, contains the opacity value of the color object.

## Discussion

If `NULL` is passed in as an argument, the method doesn’t set that value. This method works only with objects representing colors in the calibratedWhite, NSCalibratedBlackColorSpace, NSDeviceBlackColorSpace, or deviceWhite color space. Sending it to other objects raises an exception.

## See Also

### Related Documentation

class NSColor

An object that stores color data and sometimes opacity (alpha value).

### Retrieving Component Values from Color Objects

func getCyan(UnsafeMutablePointer&lt;CGFloat>?, magenta: UnsafeMutablePointer&lt;CGFloat>?, yellow: UnsafeMutablePointer&lt;CGFloat>?, black: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s CMYK and opacity values.

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s HSB component and opacity values in the respective arguments.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s RGB component and opacity values in the respective arguments.

var numberOfComponents: Int

The number of components in the color.

func getComponents(UnsafeMutablePointer&lt;CGFloat>)

Returns the components of the color as an array.

