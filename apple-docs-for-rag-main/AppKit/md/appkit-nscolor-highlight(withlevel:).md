

- AppKit
- NSColor
-  highlight(withLevel:) 

Instance Method

# highlight(withLevel:)

Creates a new color object that represents a blend between the current color and the highlight color.

macOS

``` source
func highlight(withLevel val: CGFloat) -> NSColor?
```

## Parameters 

`val`  

The amount of the highlight color that is blended with the receiver’s color. This should be a number from `0.0` through `1.0`. A `highlightLevel` below `0.0` is interpreted as `0.0`; a `highlightLevel` above `1.0` is interpreted as `1.0`.

## Return Value

The new `NSColor` object. Returns `nil` if the colors can’t be converted.

## Discussion

The highlight color is provided by the highlightColor property. Call this method when you want to brighten the current color for use in highlights.

## See Also

### Transforming Existing Color Objects

func usingColorSpace(NSColorSpace) -> NSColor?

Creates a new color object representing the color of the current color object in the specified color space.

func blended(withFraction: CGFloat, of: NSColor) -> NSColor?

Creates a new color object whose component values are a weighted sum of the current color object and the specified color object’s.

func withAlphaComponent(CGFloat) -> NSColor

Creates a new color object that has the same color space and component values as the current color object, but the specified alpha component.

func shadow(withLevel: CGFloat) -> NSColor?

Creates a new color object that represents a blend between the current color and the shadow color.

func usingColorSpaceName(NSColorSpaceName) -> NSColor?

Creates a new color object whose color is the same as the receiver’s, except that the new color object is in the specified color space.

Deprecated

func usingColorSpaceName(NSColorSpaceName?, device: [NSDeviceDescriptionKey : Any]?) -> NSColor?

Creates a new color object for the same color, but in the specified color space and specific to the provided device.

Deprecated

