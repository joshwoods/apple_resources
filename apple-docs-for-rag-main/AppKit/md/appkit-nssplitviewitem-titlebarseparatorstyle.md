

- AppKit
- NSSplitViewItem
-  titlebarSeparatorStyle 

Instance Property

# titlebarSeparatorStyle

The type of separator that the app displays between the title bar and content of a window.

macOS 11.0+

``` source
var titlebarSeparatorStyle: NSTitlebarSeparatorStyle { get set }
```

## Discussion

To apply this value, you must associate the item’s view with its own title bar section. The default value is NSTitlebarSeparatorStyle.automatic. The containing window’s preference can override this preference.

## See Also

### Customizing Appearance

var allowsFullHeightLayout: Bool

A Boolean value that indicates whether full-height sidebars appear in the window after you set a style mask.

enum NSTitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

