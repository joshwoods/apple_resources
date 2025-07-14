

- UIKit
- UIColor
-  accessibilityName 

Instance Property

# accessibilityName

A localized description of the color for accessibility attributes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
var accessibilityName: String { get }
```

## See Also

### Getting the color information

Determining color values with color spaces

Change the system’s interpretation of a color value for display by selecting a color space.

var cgColor: CGColor

The Quartz color that corresponds to the color object.

var ciColor: CIColor

The Core Image color that corresponds to the color object.

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the HSB color space.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the RGB color space.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the grayscale components of the color.

