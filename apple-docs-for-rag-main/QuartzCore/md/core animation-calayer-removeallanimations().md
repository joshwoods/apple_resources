

- Core Animation
- CALayer
-  removeAllAnimations() 

Instance Method

# removeAllAnimations()

Remove all animations attached to the layer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func removeAllAnimations()
```

## See Also

### Layer Animations

func add(CAAnimation, forKey: String?)

Add the specified animation object to the layer’s render tree.

func animation(forKey: String) -> CAAnimation?

Returns the animation object with the specified identifier.

func removeAnimation(forKey: String)

Remove the animation object with the specified key.

func animationKeys() -> [String]?

Returns an array of strings that identify the animations currently attached to the layer.

