

- AppKit
- NSTextSelectionNavigation
- NSTextSelectionNavigation.Modifier
-  multiple 

Type Property

# multiple

The value that indicates the framework extends the selection visually inside the rectangular area defined by the anchor and dragged positions.

macOS 12.0+

``` source
static var multiple: NSTextSelectionNavigation.Modifier { get }
```

## Discussion

This produces an NSTextSelection per line.

## See Also

### Navigation modifier characteristics

static var extend: NSTextSelectionNavigation.Modifier

The value that indicates the framework extends the selection by not moving the initial location while in a drag selection.

static var visual: NSTextSelectionNavigation.Modifier

The value that indicates the framework extends the selection visually inside the rectangular area defined by the anchor and drag positions.

