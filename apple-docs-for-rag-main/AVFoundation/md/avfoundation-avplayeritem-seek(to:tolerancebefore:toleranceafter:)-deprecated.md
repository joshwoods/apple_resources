

- AVFoundation
- AVPlayerItem
-  seek(to:toleranceBefore:toleranceAfter:) Deprecated

Instance Method

# seek(to:toleranceBefore:toleranceAfter:)

Sets the current playback time within a specified time bound.

iOS 4.0–11.0DeprecatediPadOS 4.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0–11.0Deprecated

``` source
@MainActor
func seek(
    to time: CMTime,
    toleranceBefore: CMTime,
    toleranceAfter: CMTime
)
```

Deprecated

Use seek(to:toleranceBefore:toleranceAfter:completionHandler:) instead.

## Parameters 

`time`  

The time to which you would like to move the playback cursor.

`toleranceBefore`  

The tolerance allowed before `time`.

`toleranceAfter`  

The tolerance allowed after `time`.

## Discussion

The time seeked to will be within the range `[time-beforeTolerance, time+afterTolerance]`, and may differ from the specified time for efficiency. If you pass `kCMTimeZero` for both `toleranceBefore` and `toleranceAfter` (to request sample accurate seeking), you may incur additional decoding delay that impacts seeking performance.

Passing `kCMTimePositiveInfinity` for both `toleranceBefore` and `toleranceAfter` is the same as messaging seek(to:) directly.

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

func seek(to: Date) async -> Bool

Sets the current playback time to the time specified by the date object.

Deprecated

func seek(to: Date) -> Bool

Sets the current playback time to the time specified by the date object.

Deprecated

