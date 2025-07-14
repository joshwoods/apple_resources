

- SceneKit
- SCNAnimatable
-  removeAllAnimations() 

Instance Method

# removeAllAnimations()

Removes all the animations currently attached to the object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeAllAnimations()
```

**Required**

## See Also

### Managing Animations

func addAnimation(any SCNAnimationProtocol, forKey: String?)

Adds an animation object for the specified key.

**Required**

func animation(forKey: String) -> CAAnimation?

Returns the animation with the specified key.

**Required**

Deprecated

var animationKeys: [String]

An array containing the keys of all animations currently attached to the object.

**Required**

func removeAnimation(forKey: String)

Removes the animation attached to the object with the specified key.

**Required**

func removeAnimation(forKey: String, fadeOutDuration: CGFloat)

Removes the animation attached to the object with the specified key, smoothly transitioning out of the animation’s effect.

**Required**

Deprecated

