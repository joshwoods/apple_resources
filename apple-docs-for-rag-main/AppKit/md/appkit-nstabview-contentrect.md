

- AppKit
- NSTabView
-  contentRect 

Instance Property

# contentRect

The rectangle describing the content area of the tab view.

macOS

``` source
@MainActor
var contentRect: NSRect { get }
```

## Discussion

This area does not include the space required for the tab view’s tabs or borders (if any).

## See Also

### Determining the Size

var minimumSize: NSSize

The minimum size necessary for the tab view to display tabs in a useful way.

var controlSize: NSControl.ControlSize

The size of the tab view.

