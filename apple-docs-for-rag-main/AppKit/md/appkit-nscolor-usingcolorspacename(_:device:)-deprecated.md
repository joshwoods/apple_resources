

- AppKit
- NSColor
-  usingColorSpaceName(\_:device:) Deprecated

Instance Method

# usingColorSpaceName(\_:device:)

Creates a new color object for the same color, but in the specified color space and specific to the provided device.

macOS 10.0–10.14Deprecated

``` source
func usingColorSpaceName(
    _ name: NSColorSpaceName?,
    device deviceDescription: [NSDeviceDescriptionKey : Any]?
) -> NSColor?
```

Deprecated

Use -colorUsingType: or -colorUsingColorSpace: instead

## Parameters 

`name`  

The name of the color space containing the new `NSColor` object. If `colorSpace` is `nil`, the most appropriate color space is used.

`deviceDescription`  

The device description. Device descriptions can be obtained from windows, screens, and printers with the `deviceDescription` method.

If `deviceDescription` is `nil`, the current device (as obtained from the currently lockFocus’ed view’s window or, if printing, the current printer) is used.

## Return Value

The new NSColor object or `nil` if the specified conversion cannot be done.

## See Also

### Related Documentation

var colorSpaceName: NSColorSpaceName

The name of the color space associated with the color.

Deprecated

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

