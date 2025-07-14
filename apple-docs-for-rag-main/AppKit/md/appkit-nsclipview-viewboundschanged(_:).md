

- AppKit
- NSClipView
-  viewBoundsChanged(\_:) 

Instance Method

# viewBoundsChanged(\_:)

Handles an boundsDidChangeNotification, passed in the `aNotification` argument, by updating a containing NSScrollView based on the new bounds.

macOS

``` source
@MainActor
func viewBoundsChanged(_ notification: Notification)
```

## See Also

### Overriding NSView Methods

func viewFrameChanged(Notification)

Handles an frameDidChangeNotification, passed in the `aNotification` argument, by updating a containing NSScrollView based on the new frame.

