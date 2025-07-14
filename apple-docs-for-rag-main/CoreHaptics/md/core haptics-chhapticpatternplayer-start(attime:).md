

- Core Haptics
- CHHapticPatternPlayer
-  start(atTime:) 

Instance Method

# start(atTime:)

Starts playing the pattern at the specified time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func start(atTime time: TimeInterval) throws
```

**Required**

## Parameters 

`time`  

The time from which to start playing the pattern.

## Mentioned in 

Playing a single-tap haptic pattern

## Discussion

If `time` is `0` or any value less than the haptic engine’s currentTime, the pattern starts playing immediately. If you call this method on a player that’s already playing, it restarts itself at the beginning of the pattern.

## See Also

### Starting and Stopping Playback

func stop(atTime: TimeInterval) throws

Stops playing the pattern at the specified time.

**Required**

func cancel() throws

Stops the pattern player immediately and returns the specified error.

**Required**

