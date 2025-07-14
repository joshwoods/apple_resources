

- AppKit
- NSGroupTouchBarItem
-  groupUserInterfaceLayoutDirection 

Instance Property

# groupUserInterfaceLayoutDirection

The user interface direction that controls the layout order of the items.

macOS 10.13+

``` source
@MainActor
var groupUserInterfaceLayoutDirection: NSUserInterfaceLayoutDirection { get set }
```

## Discussion

The default value is NSUserInterfaceLayoutDirection.leftToRight.

If you want the order of the items in the group to respect the user’s preferred layout, set this property to the value of userInterfaceLayoutDirection on the NSApplication.

## See Also

### Configuring groups

var groupTouchBar: NSTouchBar

A bar that holds this group’s items.

