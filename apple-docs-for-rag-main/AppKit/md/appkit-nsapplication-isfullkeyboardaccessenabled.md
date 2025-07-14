

- AppKit
- NSApplication
-  isFullKeyboardAccessEnabled 

Instance Property

# isFullKeyboardAccessEnabled

A Boolean value indicating whether Full Keyboard Access is enabled in the Keyboard preference pane.

macOS 10.6+

``` source
@MainActor
var isFullKeyboardAccessEnabled: Bool { get }
```

## Discussion

The value of this property is true if Full Keyboard Access is enabled or false if it’s not. You might use this value to implement your own key loop or to implement in-control tabbing behavior similar to NSTableView. Because of the nature of the preference storage, you won’t be notified of changes to this property if you attempt to observe it through key-value observing; however, accessing this property is fairly inexpensive, so you can access it directly rather than caching it.

