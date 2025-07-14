

- AppKit
- NSMenu
-  menuChangedMessagesEnabled Deprecated

Instance Property

# menuChangedMessagesEnabled

Indicates whether messages are sent to the application’s windows each time the menu changes.

macOS 10.0–10.11Deprecated

``` source
var menuChangedMessagesEnabled: Bool { get set }
```

## Discussion

This property indicates whether messages are sent to the application’s windows each time the menu changes.

To avoid the “flickering” effect of many successive menu changes, set the value of this property to false, make changes to the menu, and then set the value of this property to true. This approach has the effect of batching changes and applying them all at once.

### Special Considerations

In macOS 10.6 and later this property has no effect.

