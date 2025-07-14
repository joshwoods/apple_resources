

- UIKit
- UIColor
-  ciColor 

Instance Property

# ciColor

The Core Image color that corresponds to the color object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var ciColor: CIColor { get }
```

## Discussion

This property throws an exception if the color object wasn’t initialized with a Core Image color.

The color object in this property doesn’t adapt automatically to Dark Mode changes. If you use it to set the color of interface elements, you must update that color yourself. You update that color when the userInterfaceStyle trait of the current trait collection changes.

For information on how to apply color information reliably, see Supporting Dark Mode in Your Interface.

## See Also

### Getting the color information

Determining color values with color spaces

Change the system’s interpretation of a color value for display by selecting a color space.

var cgColor: CGColor

The Quartz color that corresponds to the color object.

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the HSB color space.

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the components that form the color in the RGB color space.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?) -> Bool

Returns the grayscale components of the color.

var accessibilityName: String

A localized description of the color for accessibility attributes.

