

- AppKit
- NSApplication
-  setWindowsNeedUpdate(\_:) 

Instance Method

# setWindowsNeedUpdate(\_:)

Sets whether the receiver’s windows need updating when the receiver has finished processing the current event.

macOS

``` source
@MainActor
func setWindowsNeedUpdate(_ needUpdate: Bool)
```

## Parameters 

`needUpdate`  

If true, the receiver’s windows are updated after an event is processed.

## Discussion

This method is especially useful for making sure menus are updated to reflect changes not initiated by user actions, such as messages received from remote objects.

## See Also

### Updating Windows

func updateWindows()

Sends an update() message to each onscreen window.

