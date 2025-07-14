

- AppKit
-  NSColor 

Class

# NSColor

An object that stores color data and sometimes opacity (alpha value).

macOS

``` source
class NSColor
```

## Overview

Many methods in AppKit require you to specify color data using an NSColor object; when drawing you use them to set the current fill and stroke colors. Color objects are immutable and thread-safe. You can create color objects in many ways:

- Load colors from an asset catalog. Colors created from assets can adapt automatically to system appearance changes.

- Use the semantic colors for custom UI elements, so that they match the appearance of other AppKit views; see UI Element Colors.

- Use the adaptable system colors, such as systemBlue, when you want a specific tint that looks correct in both light and dark environments.

- Create a color object from another object, such as a Core Graphics representation of a color, or a Core Image color.

- Create a color from an NSImage object, and paint a repeating pattern instead of using a solid color.

- Create a color by applying a transform to another NSColor object. For example, you might perform a blend operation between two colors, or you might create a color that represents the same color, but in a different color space.

- Create custom colors using raw component values, and a variety of color spaces, when you need to represent user-specified colors.

For user-specified colors, you can also display a color panel and let the user specify the color. For information about color panels, see NSColorPanel.

### Color and Color Spaces

A color object is typically represented internally as a Core Graphics color (CGColor) in a Core Graphics color space (CGColorSpace). Colors can also be created in extended color spaces:

- extendedSRGB

- extendedGenericGamma22Gray

When you need to worry about color spaces, use extended color spaces as working color spaces. When you need to worry about representing that color as closely as possible in a specific color space, convert the color from the extended color space into the target color space.

When working in an extended color space, color values are not clamped to fit inside the color gamut, meaning that component values may be less than `0.0` or greater than `1.0`. When displayed on an sRGB display, such colors are outside the gamut and won’t render accurately. However, extended color spaces are useful as working color spaces when you want a pixel format and representation that other color spaces can be easily converted into. For example, a color in the Display P3 color space can convert to an extended sRGB format, even if it isn’t within the sRGB color gamut. While some of the converted color’s values are outside of the 0-1.0 range, the color renders correctly when viewed on a device with a P3 display gamut.

It is a programmer error to access color components of a color space that the `NSColor` object does not support. For example, you cannot access the redComponent property and getRed(_:green:blue:alpha:) method on a color that uses the CMYK color space. Further, the getComponents(_:) method and numberOfComponents property work only in color spaces that have individual components. As such, they return the components of color objects as individual floating-point values regardless of whether they’re based on NSColorSpace objects or named color spaces. However, older component-fetching methods such as getRed(_:green:blue:alpha:) are effective only on color objects based on named color spaces.

If you have a color object in an unknown color space and you want to extract its components, convert the color object to a known color space and then use the component accessor methods of that color space.

For design guidance, see Human Interface Guidelines.

## Topics

### Getting and Creating Colors

Get one of the AppKit-defined colors, load colors from asset catalogs, or create custom colors for your app.

UI Element Colors

Retrieve standard color objects for use with windows, controls, labels, text, selections and other content in your app.

Standard Colors

Retrieve the standard color objects for common colors like red, blue, green, black, white, and more.

Color Creation

Load colors from asset catalogs, and create colors from raw component values, such as those used by grayscale, RGB, HSB, and CMYK colors.

### Applying Specific Appearances to Colors

func withSystemEffect(NSColor.SystemEffect) -> NSColor

Returns a new color object that represents the current color modified to include the specified visual effect.

enum SystemEffect

Constants for user interactions that change the appearance of a view or control.

### Transforming Existing Color Objects

func usingColorSpace(NSColorSpace) -> NSColor?

Creates a new color object representing the color of the current color object in the specified color space.

func blended(withFraction: CGFloat, of: NSColor) -> NSColor?

Creates a new color object whose component values are a weighted sum of the current color object and the specified color object’s.

func withAlphaComponent(CGFloat) -> NSColor

Creates a new color object that has the same color space and component values as the current color object, but the specified alpha component.

func highlight(withLevel: CGFloat) -> NSColor?

Creates a new color object that represents a blend between the current color and the highlight color.

func shadow(withLevel: CGFloat) -> NSColor?

Creates a new color object that represents a blend between the current color and the shadow color.

func usingColorSpaceName(NSColorSpaceName) -> NSColor?

Creates a new color object whose color is the same as the receiver’s, except that the new color object is in the specified color space.

Deprecated

func usingColorSpaceName(NSColorSpaceName?, device: [NSDeviceDescriptionKey : Any]?) -> NSColor?

Creates a new color object for the same color, but in the specified color space and specific to the provided device.

Deprecated

### Determining the Alpha Support of Colors

class var ignoresAlpha: Bool

A Boolean value that indicates whether the app supports alpha.

Deprecated

### Copying and Pasting Color Information

init?(from: NSPasteboard)

Creates a color object from color data currently on the pasteboard.

func write(to: NSPasteboard)

Writes the color object’s data to the specified pasteboard.

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

func getComponents(UnsafeMutablePointer&lt;CGFloat>)

Returns the components of the color as an array.

### Retrieving Individual Components

var alphaComponent: CGFloat

The alpha (opacity) component value of the color.

var whiteComponent: CGFloat

The white component value of the color.

var redComponent: CGFloat

The red component value of the color.

var greenComponent: CGFloat

The green component value of the color.

var blueComponent: CGFloat

The blue component value of the color.

var cyanComponent: CGFloat

The cyan component value of the color.

var magentaComponent: CGFloat

The magenta component value of the color.

var yellowComponent: CGFloat

The yellow component value of the color.

var blackComponent: CGFloat

The black component value of the color.

var hueComponent: CGFloat

The hue component value of the color.

var saturationComponent: CGFloat

The saturation component value of the color.

var brightnessComponent: CGFloat

The brightness component value of the color.

var catalogNameComponent: NSColorList.Name

The catalog containing the color’s name.

var localizedCatalogNameComponent: String

The localized version of the catalog name containing the color.

var colorNameComponent: NSColor.Name

The name of the color.

var localizedColorNameComponent: String

The localized version of the color name.

### Working with the Color Space

var type: NSColor.ColorType

The type of the color object.

func usingType(NSColor.ColorType) -> NSColor?

Returns a version of the color object that is compatible with the specified color type.

enum ColorType

Constants that indicate the color’s type, and which methods may be called on the color object.

var colorSpace: NSColorSpace

The color space associated with the color.

var colorSpaceName: NSColorSpaceName

The name of the color space associated with the color.

Deprecated

struct NSColorSpaceName

Constants that specify color space names.

### Retrieving Core Graphics Color Information

var cgColor: CGColor

The Core Graphics color object corresponding to the color.

### Drawing with Colors

func drawSwatch(in: NSRect)

Draws the current color in the specified rectangle.

func set()

Sets the color of subsequent drawing to the color that the color object represents.

func setFill()

Sets the fill color of subsequent drawing to the color object’s color.

func setStroke()

Sets the stroke color of subsequent drawing to the color object’s color.

### Determining When Colors Change

class let systemColorsDidChangeNotification: NSNotification.Name

Sent when the system colors have changed, such as through a system control panel interface.

class let currentControlTintDidChangeNotification: NSNotification.Name

Sent after the user changes control tint preference.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityColor
- NSCoding
- NSCopying
- NSObjectProtocol
- NSPasteboardReading
- NSPasteboardWriting
- NSSecureCoding
- Sendable
- Transferable

## See Also

### Colors

class NSColorList

An ordered list of color objects, identified by keys.

class NSColorSpace

An object that represents a custom color space.

