

- AppKit
- NSView
-  addGestureRecognizer(\_:) 

Instance Method

# addGestureRecognizer(\_:)

Attaches a gesture recognizer to the view.

macOS 10.10+

``` source
@MainActor
func addGestureRecognizer(_ gestureRecognizer: NSGestureRecognizer)
```

## Parameters 

`gestureRecognizer`  

The gesture recognizer to attach to the view. This parameter must not be `nil`.

## Discussion

Attaching a gesture recognizer to a view defines the scope of the represented gesture, causing it to receive touches occurring only in the view or one of its subviews. The view establishes a strong reference to the specified gesture recognizer.

## See Also

### Managing Gesture Recognizers

var gestureRecognizers: [NSGestureRecognizer]

The gesture recognize objects currently attached to the view.

func removeGestureRecognizer(NSGestureRecognizer)

Detaches a gesture recognizer from the view.

