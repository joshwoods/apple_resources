

- AppKit
- NSTabView
-  minimumSize 

Instance Property

# minimumSize

The minimum size necessary for the tab view to display tabs in a useful way.

macOS

``` source
@MainActor
var minimumSize: NSSize { get }
```

## Discussion

You can use the value of this property to limit how much a user can resize a tab view.

## See Also

### Related Documentation

var tabViewType: NSTabView.TabType

The tab type to display the tabs.

### Determining the Size

var contentRect: NSRect

The rectangle describing the content area of the tab view.

var controlSize: NSControl.ControlSize

The size of the tab view.

