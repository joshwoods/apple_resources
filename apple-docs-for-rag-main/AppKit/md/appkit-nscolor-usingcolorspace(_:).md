

- AppKit
- NSColor
-  usingColorSpace(\_:) 

Instance Method

# usingColorSpace(\_:)

Creates a new color object representing the color of the current color object in the specified color space.

macOS

``` source
func usingColorSpace(_ space: NSColorSpace) -> NSColor?
```

## Parameters 

`space`  

The color space of the new `NSColor` object.

## Return Value

The new `NSColor` object. This method converts the receiver’s color to an equivalent one in the new color space. Although the new color might have different component values, it looks the same as the original. Returns `nil` if conversion is not possible.

## Discussion

If the receiver’s color space is the same as that specified in `space`, this method returns the same `NSColor` object.

## See Also

### Related Documentation

init(colorSpace: NSColorSpace, components: UnsafePointer&lt;CGFloat>, count: Int)

Creates a color object from the specified components of the given color space.

### Transforming Existing Color Objects

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

