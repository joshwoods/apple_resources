

- AppKit
- NSSplitViewItem
-  allowsFullHeightLayout 

Instance Property

# allowsFullHeightLayout

A Boolean value that indicates whether full-height sidebars appear in the window after you set a style mask.

macOS 11.0+

``` source
var allowsFullHeightLayout: Bool { get set }
```

## Discussion

This property only applies to NSSplitViewItem.Behavior.sidebar and NSSplitViewItem.Behavior.inspector. The default value is true.

## See Also

### Customizing Appearance

var titlebarSeparatorStyle: NSTitlebarSeparatorStyle

The type of separator that the app displays between the title bar and content of a window.

enum NSTitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

