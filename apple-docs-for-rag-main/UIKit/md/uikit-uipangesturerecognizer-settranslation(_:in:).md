

- UIKit
- UIPanGestureRecognizer
-  setTranslation(\_:in:) 

Instance Method

# setTranslation(\_:in:)

Sets the translation value in the coordinate system of the specified view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setTranslation(
    _ translation: CGPoint,
    in view: UIView?
)
```

## Parameters 

`translation`  

A point that identifies the new translation value.

`view`  

A view in whose coordinate system the translation is to occur.

## Discussion

Changing the translation value resets the velocity of the pan.

## See Also

### Tracking the location and velocity of the gesture

func translation(in: UIView?) -> CGPoint

Interprets the pan gesture in the coordinate system of the specified view.

func velocity(in: UIView?) -> CGPoint

Interprets the velocity of the pan gesture in the coordinate system of the specified view.

