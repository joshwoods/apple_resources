

- SceneKit
- SCNAnimatable
-  isAnimationPaused(forKey:) Deprecated

Instance Method

# isAnimationPaused(forKey:)

Returns a Boolean value indicating whether the animation attached to the object with the specified key is paused.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
func isAnimationPaused(forKey key: String) -> Bool
```

**Required**

Deprecated

Use -\[SCNAnimationPlayer paused\] instead

## Parameters 

`key`  

A string identifying an attached animation.

## Return Value

true if the specified animation is paused. false if the animation is running or no animation is attached to the object with that key.

## See Also

### Pausing and Resuming Animations

func pauseAnimation(forKey: String)

Pauses the animation attached to the object with the specified key.

**Required**

Deprecated

func resumeAnimation(forKey: String)

Resumes a previously paused animation attached to the object with the specified key.

**Required**

Deprecated

