

- UIKit
- UIView
-  addMotionEffect(\_:) 

Instance Method

# addMotionEffect(\_:)

Begins applying a motion effect to the view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addMotionEffect(_ effect: UIMotionEffect)
```

## Parameters 

`effect`  

The motion effect.

## Discussion

The system animates the transition to the motion effect’s values using the present UIView animation context. The motion effect’s keyPath/value pairs are applied to the view’s presentation layer.

## See Also

### Using motion effects

var motionEffects: [UIMotionEffect]

The array of motion effects for the view.

func removeMotionEffect(UIMotionEffect)

Stops applying a motion effect to the view.

