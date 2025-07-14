

- Core Haptics
- CHHapticAdvancedPatternPlayer
-  pause(atTime:) 

Instance Method

# pause(atTime:)

Pauses the haptic player during playback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func pause(atTime time: TimeInterval) throws
```

**Required**

## Parameters 

`time`  

The time in the haptic pattern at which to pause playback.

## See Also

### Controlling Playback

func resume(atTime: TimeInterval) throws

Resumes playing a paused haptic.

**Required**

func seek(toOffset: TimeInterval) throws

Jumps to the specified offset time in playing the haptic.

**Required**

