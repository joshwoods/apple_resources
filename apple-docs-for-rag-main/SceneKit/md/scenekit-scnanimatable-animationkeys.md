

- SceneKit
- SCNAnimatable
-  animationKeys 

Instance Property

# animationKeys

An array containing the keys of all animations currently attached to the object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var animationKeys: [String] { get }
```

**Required**

## Discussion

This array contains all keys for which animations are attached to the object, or is empty if there are no attached animations. The ordering of animation keys in the array is arbitrary.

## See Also

### Managing Animations

func addAnimation(any SCNAnimationProtocol, forKey: String?)

Adds an animation object for the specified key.

**Required**

func animation(forKey: String) -> CAAnimation?

Returns the animation with the specified key.

**Required**

Deprecated

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

