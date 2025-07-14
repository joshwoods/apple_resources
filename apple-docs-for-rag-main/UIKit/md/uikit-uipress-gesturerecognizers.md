

- UIKit
- UIPress
-  gestureRecognizers 

Instance Property

# gestureRecognizers

The gesture recognizers that are receiving the press.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var gestureRecognizers: [UIGestureRecognizer]? { get }
```

## Discussion

The objects held in this array are instances of a subclass of the abstract base class, UIGestureRecognizer. If there are no gesture recognizers currently receiving the touch objects, this property holds an empty array.

## See Also

### Getting a press object’s gesture recognizers

var force: CGFloat

The force of the button press.

