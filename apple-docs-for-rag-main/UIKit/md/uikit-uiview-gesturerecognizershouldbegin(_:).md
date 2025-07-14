

- UIKit
- UIView
-  gestureRecognizerShouldBegin(\_:) 

Instance Method

# gestureRecognizerShouldBegin(\_:)

Asks the view if the gesture recognizer should continue tracking touch events.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func gestureRecognizerShouldBegin(_ gestureRecognizer: UIGestureRecognizer) -> Bool
```

## Parameters 

`gestureRecognizer`  

The gesture recognizer that’s attempting to transition out of the UIGestureRecognizer.State.possible state.

## Return Value

true if the gesture recognizer should continue tracking touch events and use them to trigger a gesture or false if it should transition to the UIGestureRecognizer.State.failed state.

## Discussion

Subclasses may override this method and use it to prevent the recognition of particular gestures. For example, the UISlider class uses this method to prevent swipes parallel to the slider’s travel direction and that start in the thumb.

At the time this method is called, the gesture recognizer is in the UIGestureRecognizer.State.possible state and thinks it has the events needed to move to the UIGestureRecognizer.State.began state.

The default implementation of this method returns true.

Note

In iOS 17, Messages allows you to interactively resize iMessage apps with a vertical pan gesture. Messages handles any conflicts between resize gestures and your custom gestures. If your app uses manual touch handling, override those methods in your app’s UIView. You can either change your manual touch handling code to use a gesture recognizer instead, or your UIView can override gestureRecognizerShouldBegin(_:) and return NO when your iMessage app doesn’t own the gesture.

## See Also

### Managing gesture recognizers

func addGestureRecognizer(UIGestureRecognizer)

Attaches a gesture recognizer to the view.

func removeGestureRecognizer(UIGestureRecognizer)

Detaches a gesture recognizer from the receiving view.

var gestureRecognizers: [UIGestureRecognizer]?

The gesture-recognizer objects currently attached to the view.

