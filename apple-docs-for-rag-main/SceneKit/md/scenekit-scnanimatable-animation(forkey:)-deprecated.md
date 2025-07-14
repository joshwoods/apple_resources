

- SceneKit
- SCNAnimatable
-  animation(forKey:) Deprecated

Instance Method

# animation(forKey:)

Returns the animation with the specified key.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func animation(forKey key: String) -> CAAnimation?
```

**Required**

## Parameters 

`key`  

A string identifying a previously added animation.

## Return Value

An animation object matching the key, or `nil` if no such animation exists.

## Discussion

Attempting to modify any properties of the returned object results in undefined behavior.

## See Also

### Managing Animations

func addAnimation(any SCNAnimationProtocol, forKey: String?)

Adds an animation object for the specified key.

**Required**

var animationKeys: [String]

An array containing the keys of all animations currently attached to the object.

**Required**

func removeAllAnimations()

Removes all the animations currently attached to the object.

**Required**

func removeAnimation(forKey: String)

Removes the animation attached to the object with the specified key.

**Required**

func removeAnimation(forKey: String, fadeOutDuration: CGFloat)

Removes the animation attached to the object with the specified key, smoothly transitioning out of the animation’s effect.

**Required**

Deprecated

