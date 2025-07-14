

- UIKit
- UIInterpolatingMotionEffect
-  init(keyPath:type:) 

Initializer

# init(keyPath:type:)

Initializes and returns an interpolating motion effect object configured for the specific tilt direction.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    keyPath: String,
    type: UIInterpolatingMotionEffect.EffectType
)
```

## Parameters 

`keyPath`  

The key path of the view that you want to modify. This path must correspond to an animatable property of the view on which this motion effect is applied. For example, to update the center property of the view, specify the string “center”.

`type`  

The type of motion to track. You can track horizontal or vertical tilt. For a list of possible values, see UIInterpolatingMotionEffect.EffectType.

## Return Value

An initialized interpolating motion effect object.

## See Also

### Initializing a motion effect

init?(coder: NSCoder)

Creates a motion effect from data in an unarchiver.

