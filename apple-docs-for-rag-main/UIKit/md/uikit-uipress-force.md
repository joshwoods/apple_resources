

- UIKit
- UIPress
-  force 

Instance Property

# force

The force of the button press.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var force: CGFloat { get }
```

## Discussion

While all buttons can be “down” or “up”, some physical buttons also have a notion of a “force” with which they’re pressed. For analog buttons, force returns a value between 0 and 1, and for digital buttons it returns 0 or 1.

## See Also

### Getting a press object’s gesture recognizers

var gestureRecognizers: [UIGestureRecognizer]?

The gesture recognizers that are receiving the press.

