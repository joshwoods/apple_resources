

- AppKit
- NSColor
-  withAlphaComponent(\_:) 

Instance Method

# withAlphaComponent(\_:)

Creates a new color object that has the same color space and component values as the current color object, but the specified alpha component.

macOS

``` source
func withAlphaComponent(_ alpha: CGFloat) -> NSColor
```

## Parameters 

`alpha`  

The opacity value of the new `NSColor` object.

## Return Value

The new `NSColor` object. If the receiver’s color space doesn’t include an alpha component, the receiver is returned.

## Discussion

A subclass with explicit opacity components should override this method to return a color with the specified alpha.

## See Also

### Related Documentation

var alphaComponent: CGFloat

The alpha (opacity) component value of the color.

### Transforming Existing Color Objects

func usingColorSpace(NSColorSpace) -> NSColor?

Creates a new color object representing the color of the current color object in the specified color space.

func blended(withFraction: CGFloat, of: NSColor) -> NSColor?

Creates a new color object whose component values are a weighted sum of the current color object and the specified color object’s.

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

