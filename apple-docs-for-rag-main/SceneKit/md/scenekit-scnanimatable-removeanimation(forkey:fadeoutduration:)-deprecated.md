

- SceneKit
- SCNAnimatable
-  removeAnimation(forKey:fadeOutDuration:) Deprecated

Instance Method

# removeAnimation(forKey:fadeOutDuration:)

Removes the animation attached to the object with the specified key, smoothly transitioning out of the animation’s effect.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
func removeAnimation(
    forKey key: String,
    fadeOutDuration duration: CGFloat
)
```

**Required**

## Parameters 

`key`  

A string identifying an attached animation to remove.

`duration`  

The duration for transitioning out of the animation’s effect before it is removed.

## Discussion

Use this method to create smooth transitions between the effects of multiple animations. For example, the geometry loaded from a scene file for a game character may have associated animations for player actions such as walking and jumping. When the player lands from a jump, you remove the jump animation so the character continues walking. If you use the removeAnimation(forKey:) method to remove the jump animation, SceneKit abruptly switches from the current frame of the jump animation to the current frame of the walk animation. If you use the removeAnimation(forKey:fadeOutDuration:) method instead, SceneKit plays both animations at once during that duration and interpolates vertex positions from one animation to the other, creating a smooth transition.

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

func removeAllAnimations()

Removes all the animations currently attached to the object.

**Required**

func removeAnimation(forKey: String)

Removes the animation attached to the object with the specified key.

**Required**

