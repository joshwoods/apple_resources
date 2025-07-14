

- Core Haptics
- CHHapticAdvancedPatternPlayer
-  seek(toOffset:) 

Instance Method

# seek(toOffset:)

Jumps to the specified offset time in playing the haptic.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func seek(toOffset offsetTime: TimeInterval) throws
```

**Required**

## Parameters 

`offsetTime`  

The time in the haptic pattern at which to seek playback.

## See Also

### Controlling Playback

func pause(atTime: TimeInterval) throws

Pauses the haptic player during playback.

**Required**

func resume(atTime: TimeInterval) throws

Resumes playing a paused haptic.

**Required**

