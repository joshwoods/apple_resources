

- Core Haptics
- CHHapticPatternPlayer
-  stop(atTime:) 

Instance Method

# stop(atTime:)

Stops playing the pattern at the specified time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func stop(atTime time: TimeInterval) throws
```

**Required**

## Parameters 

`time`  

The time at which to stop playing the pattern.

## Discussion

If `time` is `0` or any value less than the haptic engine’s currentTime, the pattern stops playing immediately.

## See Also

### Starting and Stopping Playback

func start(atTime: TimeInterval) throws

Starts playing the pattern at the specified time.

**Required**

func cancel() throws

Stops the pattern player immediately and returns the specified error.

**Required**

