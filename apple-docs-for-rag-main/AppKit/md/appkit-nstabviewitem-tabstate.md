

- AppKit
- NSTabViewItem
-  tabState 

Instance Property

# tabState

Returns the current display state of the tab associated with the receiver.

macOS

``` source
var tabState: NSTabViewItem.State { get }
```

## Discussion

The possible values are `NSSelectedTab`, `NSBackgroundTab`, or `NSPressedTab`. Your application does not directly set the tab state.

