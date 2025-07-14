

- AppKit
- NSColor
-  shadowColor 

Type Property

# shadowColor

The color to use for virtual shadows cast by raised objects on the screen.

macOS

``` source
class var shadowColor: NSColor { get }
```

## Return Value

The system color for the virtual shadows case by raised objects on the screen.

## Discussion

This method is invoked by shadow(withLevel:). For general information about system colors, see Accessing System Colors.

## See Also

### Related Documentation

func shadow(withLevel: CGFloat) -> NSColor?

Creates a new color object that represents a blend between the current color and the shadow color.

### Highlights and Shadows

class var findHighlightColor: NSColor

The highlight color to use for the bubble that shows inline search result values.

class var highlightColor: NSColor

The color to use as a virtual light source on the screen.

