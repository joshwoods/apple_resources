

- UIKit
- UITouch
-  gestureRecognizers 

Instance Property

# gestureRecognizers

The gesture recognizers that are receiving the touch object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var gestureRecognizers: [UIGestureRecognizer]? { get }
```

## Discussion

The objects in the array are instances of a subclass of the abstract base class UIGestureRecognizer. If there are no gesture recognizers currently receiving the touch, this property contains an empty array.

