

- AppKit
- NSApplication
-  preventWindowOrdering() 

Instance Method

# preventWindowOrdering()

Suppresses the usual window ordering in handling the most recent mouse-down event.

macOS

``` source
@MainActor
func preventWindowOrdering()
```

## Discussion

This method is only useful for mouse-down events when you want to prevent the window that receives the event from being ordered to the front.

## See Also

### Managing Window Layers

func arrangeInFront(Any?)

Arranges windows listed in the Window menu in front of all other windows.

