

- AppKit
- NSGestureRecognizer
-  touchesCancelled(with:) 

Instance Method

# touchesCancelled(with:)

Called when a system event, such as a low-memory warning, cancels an in-progress touch event in an NSTouchBar object.

macOS 10.12.2+

``` source
@MainActor
func touchesCancelled(with event: NSEvent)
```

## See Also

### Instance Methods

func touchesBegan(with: NSEvent)

Called when one or more fingers first make contact with an NSTouchBar instance on the Touch Bar.

func touchesEnded(with: NSEvent)

Called when one or more fingers are removed from contact with an NSTouchBar instance on the Touch Bar.

func touchesMoved(with: NSEvent)

Called when one or more fingers, associated with an in-progress event, move within an NSTouchBar instance on the Touch Bar.

