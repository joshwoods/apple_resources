

- SceneKit
- SCNAnimatable
-  addAnimation(\_:forKey:) 

Instance Method

# addAnimation(\_:forKey:)

Adds an animation object for the specified key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addAnimation(
    _ animation: any SCNAnimationProtocol,
    forKey key: String?
)
```

**Required**

## Parameters 

`animation`  

The animation object to be added.

`key`  

An string identifying the animation for later retrieval. You may pass `nil` if you don’t need to reference the animation later.

## Discussion

Newly added animations begin executing after the current run loop cycle ends.

SceneKit does not define any requirements for the contents of the `key` parameter—it need only be unique among the keys for other animations you add. If you add an animation with an existing key, this method overwrites the existing animation.

## See Also

### Managing Animations

func animation(forKey: String) -> CAAnimation?

Returns the animation with the specified key.

**Required**

Deprecated

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

