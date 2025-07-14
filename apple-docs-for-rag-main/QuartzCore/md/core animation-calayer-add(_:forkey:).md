

- Core Animation
- CALayer
-  add(\_:forKey:) 

Instance Method

# add(\_:forKey:)

Add the specified animation object to the layer’s render tree.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func add(
    _ anim: CAAnimation,
    forKey key: String?
)
```

## Parameters 

`anim`  

The animation to be added to the render tree. This object is copied by the render tree, not referenced. Therefore, subsequent modifications to the object are not propagated into the render tree.

`key`  

A string that identifies the animation. Only one animation per unique key is added to the layer. The special key kCATransition is automatically used for transition animations. You may specify `nil` for this parameter.

## Discussion

If the `duration` property of the animation is zero or negative, the duration is changed to the current value of the kCATransactionAnimationDuration transaction property (if set) or to the default value of `0.25` seconds.

## See Also

### Layer Animations

func animation(forKey: String) -> CAAnimation?

Returns the animation object with the specified identifier.

func removeAllAnimations()

Remove all animations attached to the layer.

func removeAnimation(forKey: String)

Remove the animation object with the specified key.

func animationKeys() -> [String]?

Returns an array of strings that identify the animations currently attached to the layer.

