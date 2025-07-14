

- UIKit
- UIGestureRecognizer
-  location(in:) 

Instance Method

# location(in:)

Returns the point computed as the location in a given view of the gesture represented by the gesture recognizer.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func location(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

A UIView object on which the gesture took place. Specify `nil` to indicate the window.

## Return Value

A point in the local coordinate system of `view` that identifies the location of the gesture. If `nil` is specified for `view`, the method returns the gesture location in the window’s base coordinate system.

## Discussion

The returned value is a generic single-point location for the gesture computed by the UIKit framework. It is usually the centroid of the touches involved in the gesture. For objects of the UISwipeGestureRecognizer and UITapGestureRecognizer classes, the location returned by this method has a significance special to the gesture. This significance is documented in the reference for those classes.

## See Also

### Getting the touches and location of a gesture

func location(ofTouch: Int, in: UIView?) -> CGPoint

Returns the location of one of the gesture’s touches in the local coordinate system of a given view.

var numberOfTouches: Int

The number of touches involved in the gesture represented by the gesture recognizer.

