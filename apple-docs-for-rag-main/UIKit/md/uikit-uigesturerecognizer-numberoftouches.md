

- UIKit
- UIGestureRecognizer
-  numberOfTouches 

Instance Property

# numberOfTouches

The number of touches involved in the gesture represented by the gesture recognizer.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var numberOfTouches: Int { get }
```

## Return Value

The number of UITouch objects in a private array maintained by the receiver. Each of these objects represents a touch in the current gesture.

## Discussion

Using the value returned by this method in a loop, you can ask for the location of individual touches using the location(ofTouch:in:) method.

## See Also

### Getting the touches and location of a gesture

func location(in: UIView?) -> CGPoint

Returns the point computed as the location in a given view of the gesture represented by the gesture recognizer.

func location(ofTouch: Int, in: UIView?) -> CGPoint

Returns the location of one of the gesture’s touches in the local coordinate system of a given view.

