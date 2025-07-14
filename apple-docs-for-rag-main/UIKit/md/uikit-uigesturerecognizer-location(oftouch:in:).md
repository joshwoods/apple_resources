

- UIKit
- UIGestureRecognizer
-  location(ofTouch:in:) 

Instance Method

# location(ofTouch:in:)

Returns the location of one of the gesture’s touches in the local coordinate system of a given view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func location(
    ofTouch touchIndex: Int,
    in view: UIView?
) -> CGPoint
```

## Parameters 

`touchIndex`  

The index of a UITouch object in a private array maintained by the receiver. This touch object represents a touch of the current gesture.

`view`  

A UIView object on which the gesture took place. Specify `nil` to indicate the window.

## Return Value

A point in the local coordinate system of `view` that identifies the location of the touch. If `nil` is specified for `view`, the method returns the touch location in the window’s base coordinate system.

## See Also

### Getting the touches and location of a gesture

func location(in: UIView?) -> CGPoint

Returns the point computed as the location in a given view of the gesture represented by the gesture recognizer.

var numberOfTouches: Int

The number of touches involved in the gesture represented by the gesture recognizer.

