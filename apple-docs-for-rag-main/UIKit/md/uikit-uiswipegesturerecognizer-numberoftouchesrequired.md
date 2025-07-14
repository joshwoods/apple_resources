

- UIKit
- UISwipeGestureRecognizer
-  numberOfTouchesRequired 

Instance Property

# numberOfTouchesRequired

The number of touches necessary for swipe recognition.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var numberOfTouchesRequired: Int { get set }
```

## Mentioned in 

Handling swipe gestures

## Discussion

The default value is `1`.

## See Also

### Configuring the gesture

var direction: UISwipeGestureRecognizer.Direction

The permitted direction of the swipe for this gesture recognizer.

struct Direction

The direction of the swipe.

