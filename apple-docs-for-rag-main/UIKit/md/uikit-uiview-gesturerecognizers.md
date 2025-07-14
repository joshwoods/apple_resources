

- UIKit
- UIView
-  gestureRecognizers 

Instance Property

# gestureRecognizers

The gesture-recognizer objects currently attached to the view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var gestureRecognizers: [UIGestureRecognizer]? { get set }
```

## Discussion

Each of these objects is an instance of a subclass of the abstract base class UIGestureRecognizer. The default value of this property is `nil`. If you add a gesture recognizer and then remove it, the value of the property is an empty array.

## See Also

### Managing gesture recognizers

func addGestureRecognizer(UIGestureRecognizer)

Attaches a gesture recognizer to the view.

func removeGestureRecognizer(UIGestureRecognizer)

Detaches a gesture recognizer from the receiving view.

func gestureRecognizerShouldBegin(UIGestureRecognizer) -> Bool

Asks the view if the gesture recognizer should continue tracking touch events.

