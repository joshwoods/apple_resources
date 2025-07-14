

- Core Animation
- CALayer
-  removeAnimation(forKey:) 

Instance Method

# removeAnimation(forKey:)

Remove the animation object with the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func removeAnimation(forKey key: String)
```

## Parameters 

`key`  

The identifier of the animation to remove.

## See Also

### Layer Animations

func add(CAAnimation, forKey: String?)

Add the specified animation object to the layer’s render tree.

func animation(forKey: String) -> CAAnimation?

Returns the animation object with the specified identifier.

func removeAllAnimations()

Remove all animations attached to the layer.

func animationKeys() -> [String]?

Returns an array of strings that identify the animations currently attached to the layer.

