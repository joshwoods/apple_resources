

- AVFoundation
- AVPlayerItemIntegratedTimeline
-  seek(to:completionHandler:) 

Instance Method

# seek(to:completionHandler:)

Seeks to a particular date in the integrated time domain.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func seek(
    to date: Date,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func seek(to date: Date) async -> Bool
```

## Parameters 

`date`  

A date represented in the integrated time domain.

`completionHandler`  

A callback the system invokes after the seek completes. It passes a Boolean value of `true` if the playhead moved to the new date.

## See Also

### Seeking

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: ((Bool) -> Void)?)

Seeks to a particular time in the integrated time domain.

