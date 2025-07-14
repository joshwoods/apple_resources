

- AppKit
- NSColor
-  usingColorSpaceName(\_:) Deprecated

Instance Method

# usingColorSpaceName(\_:)

Creates a new color object whose color is the same as the receiver’s, except that the new color object is in the specified color space.

macOS 10.0–10.14Deprecated

``` source
func usingColorSpaceName(_ name: NSColorSpaceName) -> NSColor?
```

Deprecated

Use -colorUsingType: or -colorUsingColorSpace: instead

## Parameters 

`name`  

The name of the color space containing the new `NSColor` object.

## Return Value

The new `NSColor` object or `nil` if the specified conversion cannot be done.

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

func usingColorSpaceName(NSColorSpaceName?, device: [NSDeviceDescriptionKey : Any]?) -> NSColor?

Creates a new color object for the same color, but in the specified color space and specific to the provided device.

Deprecated

