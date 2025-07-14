

- AppKit
- NSColor
-  blended(withFraction:of:) 

Instance Method

# blended(withFraction:of:)

Creates a new color object whose component values are a weighted sum of the current color object and the specified color object’s.

macOS

``` source
func blended(
    withFraction fraction: CGFloat,
    of color: NSColor
) -> NSColor?
```

## Parameters 

`fraction`  

The amount of the color to blend with the receiver’s color. The method converts `color` and a copy of the receiver to RGB, and then sets each component of the returned color to `fraction` of `color`‘s value plus 1 – `fraction` of the receiver’s.

`color`  

The color to blend with the receiver’s color.

## Return Value

The resulting color object or `nil` if the colors can’t be converted.

## See Also

### Transforming Existing Color Objects

func usingColorSpace(NSColorSpace) -> NSColor?

Creates a new color object representing the color of the current color object in the specified color space.

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

