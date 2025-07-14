

- UIKit
- UIView
-  removeGestureRecognizer(\_:) 

Instance Method

# removeGestureRecognizer(\_:)

Detaches a gesture recognizer from the receiving view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeGestureRecognizer(_ gestureRecognizer: UIGestureRecognizer)
```

## Parameters 

`gestureRecognizer`  

An object whose class descends from the UIGestureRecognizer class.

## Discussion

This method releases `gestureRecognizer` in addition to detaching it from the view.

## See Also

### Managing gesture recognizers

func addGestureRecognizer(UIGestureRecognizer)

Attaches a gesture recognizer to the view.

var gestureRecognizers: [UIGestureRecognizer]?

The gesture-recognizer objects currently attached to the view.

func gestureRecognizerShouldBegin(UIGestureRecognizer) -> Bool

Asks the view if the gesture recognizer should continue tracking touch events.

