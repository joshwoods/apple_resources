

- AVFoundation
- AVPlayerItem
-  seek(to:) Deprecated

Instance Method

# seek(to:)

Sets the current playback time to the specified time.

iOS 4.0–11.0DeprecatediPadOS 4.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0–11.0Deprecated

``` source
@MainActor
func seek(to time: CMTime)
```

Deprecated

Use seek(to:completionHandler:) instead.

## Parameters 

`time`  

The time to which to seek.

## Discussion

The time seeked to may differ from the specified time for efficiency. For sample accurate seeking see seek(to:toleranceBefore:toleranceAfter:).

## See Also

### Related Documentation

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: ((Bool) -> Void)?)

Sets the current playback time within a specified time bound and invokes the specified block when the seek operation completes or is interrupted.

func seek(to: CMTime, completionHandler: ((Bool) -> Void)?)

Sets the current playback time to the specified time.

### Seeking Through Media

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime)

Sets the current playback time within a specified time bound.

Deprecated

func seek(to: Date) async -> Bool

Sets the current playback time to the time specified by the date object.

Deprecated

func seek(to: Date) -> Bool

Sets the current playback time to the time specified by the date object.

Deprecated

