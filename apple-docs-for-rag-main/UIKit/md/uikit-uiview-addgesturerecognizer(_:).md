

- UIKit
- UIView
-  addGestureRecognizer(\_:) 

Instance Method

# addGestureRecognizer(\_:)

Attaches a gesture recognizer to the view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addGestureRecognizer(_ gestureRecognizer: UIGestureRecognizer)
```

## Parameters 

`gestureRecognizer`  

An object whose class descends from the UIGestureRecognizer class. This parameter must not be `nil`.

## Mentioned in 

Handling tap gestures

Handling rotation gestures

Handling pinch gestures

Handling swipe gestures

Handling long-press gestures

## Discussion

Attaching a gesture recognizer to a view defines the scope of the represented gesture, causing it to receive touches hit-tested to that view and all of its subviews. The view establishes a strong reference to the gesture recognizer.

## See Also

### Managing gesture recognizers

func removeGestureRecognizer(UIGestureRecognizer)

Detaches a gesture recognizer from the receiving view.

var gestureRecognizers: [UIGestureRecognizer]?

The gesture-recognizer objects currently attached to the view.

func gestureRecognizerShouldBegin(UIGestureRecognizer) -> Bool

Asks the view if the gesture recognizer should continue tracking touch events.

