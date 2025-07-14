

- UIKit
- UIPanGestureRecognizer
-  translation(in:) 

Instance Method

# translation(in:)

Interprets the pan gesture in the coordinate system of the specified view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func translation(in view: UIView?) -> CGPoint
```

## Parameters 

`view`  

The view in whose coordinate system the translation of the pan gesture should be computed. If you want to adjust a view’s location to keep it under the user’s finger, request the translation in that view’s superview’s coordinate system.

## Return Value

A point identifying the new location of a view in the coordinate system of its designated superview.

## Mentioned in 

Handling pan gestures

## Discussion

The x and y values report the total translation over time. They aren’t delta values from the last time that the translation was reported. Apply the translation value to the state of the view when the gesture is first recognized — don’t concatenate the value each time the handler is called.

## See Also

### Tracking the location and velocity of the gesture

func setTranslation(CGPoint, in: UIView?)

Sets the translation value in the coordinate system of the specified view.

func velocity(in: UIView?) -> CGPoint

Interprets the velocity of the pan gesture in the coordinate system of the specified view.

