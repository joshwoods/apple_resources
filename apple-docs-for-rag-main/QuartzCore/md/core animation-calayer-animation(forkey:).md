

- Core Animation
- CALayer
-  animation(forKey:) 

Instance Method

# animation(forKey:)

Returns the animation object with the specified identifier.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func animation(forKey key: String) -> CAAnimation?
```

## Parameters 

`key`  

A string that specifies the identifier of the animation. This string corresponds to the identifier string you passed to the add(_:forKey:) method.

## Return Value

The animation object matching the identifier, or `nil` if no such animation exists.

## Discussion

Use this method to retrieve only animation objects already associated with a layer. Modifying any properties of the returned object results in undefined behavior.

## See Also

### Layer Animations

func add(CAAnimation, forKey: String?)

Add the specified animation object to the layer’s render tree.

func removeAllAnimations()

Remove all animations attached to the layer.

func removeAnimation(forKey: String)

Remove the animation object with the specified key.

func animationKeys() -> [String]?

Returns an array of strings that identify the animations currently attached to the layer.

