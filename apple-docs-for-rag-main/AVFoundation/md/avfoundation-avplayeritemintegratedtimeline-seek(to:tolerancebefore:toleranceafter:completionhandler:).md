

- AVFoundation
- AVPlayerItemIntegratedTimeline
-  seek(to:toleranceBefore:toleranceAfter:completionHandler:) 

Instance Method

# seek(to:toleranceBefore:toleranceAfter:completionHandler:)

Seeks to a particular time in the integrated time domain.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func seek(
    to time: CMTime,
    toleranceBefore: CMTime,
    toleranceAfter: CMTime,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func seek(
    to time: CMTime,
    toleranceBefore: CMTime,
    toleranceAfter: CMTime
) async -> Bool
```

## Parameters 

`time`  

A time represented in the integrated time domain.

`toleranceBefore`  

A tolerance before the target time to allow.

`toleranceAfter`  

A tolerance after the target time to allow.

`completionHandler`  

A callback the system invokes after the seek completes. It passes a Boolean value of `true` if the playhead moved to the new time.

## See Also

### Seeking

func seek(to: Date, completionHandler: ((Bool) -> Void)?)

Seeks to a particular date in the integrated time domain.

