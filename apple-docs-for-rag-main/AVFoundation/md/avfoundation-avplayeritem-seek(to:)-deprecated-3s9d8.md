

- AVFoundation
- AVPlayerItem
-  seek(to:) Deprecated

Instance Method

# seek(to:)

Sets the current playback time to the time specified by the date object.

iOS 4.0–11.0DeprecatediPadOS 4.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0–11.0Deprecated

``` source
@MainActor
func seek(to date: Date) -> Bool
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

func seek(to: Date) async -> Bool

Sets the current playback time to the time specified by the date object.

Deprecated

