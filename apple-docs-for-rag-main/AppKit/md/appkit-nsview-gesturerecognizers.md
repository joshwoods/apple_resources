

- AppKit
- NSView
-  gestureRecognizers 

Instance Property

# gestureRecognizers

The gesture recognize objects currently attached to the view.

macOS 10.10+

``` source
@MainActor
var gestureRecognizers: [NSGestureRecognizer] { get set }
```

## Discussion

The objects in the array are concrete implementations of the `NSGestureRecognizer` class. If the view has no attached gesture recognizers, the array is empty.

## See Also

### Managing Gesture Recognizers

func addGestureRecognizer(NSGestureRecognizer)

Attaches a gesture recognizer to the view.

func removeGestureRecognizer(NSGestureRecognizer)

Detaches a gesture recognizer from the view.

