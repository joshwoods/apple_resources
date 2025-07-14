

- AVFoundation
- AVPlayerItem
-  seek(to:) Deprecated

Instance Method

# seek(to:)

Sets the current playback time to the time specified by the date object.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func seek(to date: Date) async -> Bool
```

Deprecated

Use seek(to:completionHandler:) instead.

## Parameters 

`date`  

The time to which to seek.

## Return Value

true if the playhead was moved to `date`, otherwise false.

## Discussion

For playback content that is associated with a range of dates, this method moves the playhead to point within that range. This method will fail (return false) if `date` is outside the range or if the content is not associated with a range of dates.

## See Also

### Related Documentation

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: ((Bool) -> Void)?)

Sets the current playback time within a specified time bound and invokes the specified block when the seek operation completes or is interrupted.

func seek(to: CMTime, completionHandler: ((Bool) -> Void)?)

Sets the current playback time to the specified time.

### Seeking Through Media

func seek(to: CMTime)

Sets the current playback time to the specified time.

Deprecated

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime)

Sets the current playback time within a specified time bound.

Deprecated

func seek(to: Date) -> Bool

Sets the current playback time to the time specified by the date object.

Deprecated

