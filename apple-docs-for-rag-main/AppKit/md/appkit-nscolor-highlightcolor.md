

- AppKit
- NSColor
-  highlightColor 

Type Property

# highlightColor

The color to use as a virtual light source on the screen.

macOS

``` source
class var highlightColor: NSColor { get }
```

## Return Value

The system color for the virtual light source on the screen.

## Discussion

This method is invoked by the highlight(withLevel:) method. For general information about system colors, see Accessing System Colors.

## See Also

### Related Documentation

func highlight(withLevel: CGFloat) -> NSColor?

Creates a new color object that represents a blend between the current color and the highlight color.

### Highlights and Shadows

class var findHighlightColor: NSColor

The highlight color to use for the bubble that shows inline search result values.

class var shadowColor: NSColor

The color to use for virtual shadows cast by raised objects on the screen.

