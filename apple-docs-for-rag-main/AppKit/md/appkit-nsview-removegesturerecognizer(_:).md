

- AppKit
- NSView
-  removeGestureRecognizer(\_:) 

Instance Method

# removeGestureRecognizer(\_:)

Detaches a gesture recognizer from the view.

macOS 10.10+

``` source
@MainActor
func removeGestureRecognizer(_ gestureRecognizer: NSGestureRecognizer)
```

## Parameters 

`gestureRecognizer`  

The gesture recognizer to remove. This parameter must not be `nil`.

## Discussion

Removing a gesture recognizer also removes the strong reference to it held by the view.

## See Also

### Managing Gesture Recognizers

var gestureRecognizers: [NSGestureRecognizer]

The gesture recognize objects currently attached to the view.

func addGestureRecognizer(NSGestureRecognizer)

Attaches a gesture recognizer to the view.

