

- AppKit
- NSGestureRecognizer
-  touchesMoved(with:) 

Instance Method

# touchesMoved(with:)

Called when one or more fingers, associated with an in-progress event, move within an NSTouchBar instance on the Touch Bar.

macOS 10.12.2+

``` source
@MainActor
func touchesMoved(with event: NSEvent)
```

## See Also

### Instance Methods

func touchesBegan(with: NSEvent)

Called when one or more fingers first make contact with an NSTouchBar instance on the Touch Bar.

func touchesCancelled(with: NSEvent)

Called when a system event, such as a low-memory warning, cancels an in-progress touch event in an NSTouchBar object.

func touchesEnded(with: NSEvent)

Called when one or more fingers are removed from contact with an NSTouchBar instance on the Touch Bar.

