

- SceneKit
- SCNAnimatable
-  pauseAnimation(forKey:) Deprecated

Instance Method

# pauseAnimation(forKey:)

Pauses the animation attached to the object with the specified key.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
func pauseAnimation(forKey key: String)
```

**Required**

Deprecated

Use -\[SCNAnimationPlayer setPaused:\] instead

## Parameters 

`key`  

A string identifying an attached animation.

## Discussion

This method has no effect if no animation is attached to the object with the specified key.

## See Also

### Pausing and Resuming Animations

func resumeAnimation(forKey: String)

Resumes a previously paused animation attached to the object with the specified key.

**Required**

Deprecated

func isAnimationPaused(forKey: String) -> Bool

Returns a Boolean value indicating whether the animation attached to the object with the specified key is paused.

**Required**

Deprecated

