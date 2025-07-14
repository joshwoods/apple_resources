

- UIKit
- UIPanGestureRecognizer
-  velocity(in:) 

Instance Method

# velocity(in:)

Interprets the velocity of the pan gesture in the coordinate system of the specified view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func velocity(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

The view in whose coordinate system the velocity of the pan gesture is computed.

## Return Value

The velocity of the pan gesture, which is expressed in points per second. The velocity is broken into horizontal and vertical components.

## See Also

### Tracking the location and velocity of the gesture

func translation(in: UIView?) -> CGPoint

Interprets the pan gesture in the coordinate system of the specified view.

func setTranslation(CGPoint, in: UIView?)

Sets the translation value in the coordinate system of the specified view.

