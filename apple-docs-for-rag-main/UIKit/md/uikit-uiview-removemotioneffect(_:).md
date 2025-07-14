

- UIKit
- UIView
-  removeMotionEffect(\_:) 

Instance Method

# removeMotionEffect(\_:)

Stops applying a motion effect to the view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeMotionEffect(_ effect: UIMotionEffect)
```

## Parameters 

`effect`  

The motion effect.

## Discussion

Any affected presentation values animate to their post-removal values using the present UIView animation context.

## See Also

### Using motion effects

func addMotionEffect(UIMotionEffect)

Begins applying a motion effect to the view.

var motionEffects: [UIMotionEffect]

The array of motion effects for the view.

