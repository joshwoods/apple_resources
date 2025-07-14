

- Core Haptics
- CHHapticAdvancedPatternPlayer
-  resume(atTime:) 

Instance Method

# resume(atTime:)

Resumes playing a paused haptic.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func resume(atTime time: TimeInterval) throws
```

**Required**

## Parameters 

`time`  

The time in the haptic pattern at which to resume playback.

## See Also

### Controlling Playback

func pause(atTime: TimeInterval) throws

Pauses the haptic player during playback.

**Required**

func seek(toOffset: TimeInterval) throws

Jumps to the specified offset time in playing the haptic.

**Required**

