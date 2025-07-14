

- AppKit
- NSClipView
-  viewFrameChanged(\_:) 

Instance Method

# viewFrameChanged(\_:)

Handles an frameDidChangeNotification, passed in the `aNotification` argument, by updating a containing NSScrollView based on the new frame.

macOS

``` source
@MainActor
func viewFrameChanged(_ notification: Notification)
```

## See Also

### Overriding NSView Methods

func viewBoundsChanged(Notification)

Handles an boundsDidChangeNotification, passed in the `aNotification` argument, by updating a containing NSScrollView based on the new bounds.

