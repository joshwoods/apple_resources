

- AppKit
- NSTextSelectionNavigation
- NSTextSelectionNavigation.Modifier
-  extend 

Type Property

# extend

The value that indicates the framework extends the selection by not moving the initial location while in a drag selection.

macOS 12.0+

``` source
static var extend: NSTextSelectionNavigation.Modifier { get }
```

## See Also

### Navigation modifier characteristics

static var multiple: NSTextSelectionNavigation.Modifier

The value that indicates the framework extends the selection visually inside the rectangular area defined by the anchor and dragged positions.

static var visual: NSTextSelectionNavigation.Modifier

The value that indicates the framework extends the selection visually inside the rectangular area defined by the anchor and drag positions.

