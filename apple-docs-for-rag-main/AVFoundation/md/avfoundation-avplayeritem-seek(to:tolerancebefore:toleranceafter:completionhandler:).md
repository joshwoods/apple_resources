

- AVFoundation
- AVPlayerItem
-  seek(to:toleranceBefore:toleranceAfter:completionHandler:) 

Instance Method

# seek(to:toleranceBefore:toleranceAfter:completionHandler:)

Sets the current playback time within a specified time bound and invokes the specified block when the seek operation completes or is interrupted.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func seek(
    to time: CMTime,
    toleranceBefore: CMTime,
    toleranceAfter: CMTime,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
nonisolated
func seek(
    to time: CMTime,
    toleranceBefore: CMTime,
    toleranceAfter: CMTime
) async -> Bool
```

## Parameters 

`time`  

The time to which to seek.

`toleranceBefore`  

The temporal tolerance before `time`.

Pass zero to request sample accurate seeking (this may incur additional decoding delay).

`toleranceAfter`  

The temporal tolerance after `time`.

Pass zero to request sample accurate seeking (this may incur additional decoding delay).

`completionHandler`  

The block to invoke when the seek operation has finished.

## Discussion

Use this method to seek to a specified time for the item.

The time seeked to will be within the range `[time-toleranceBefore, time+toleranceAfter]` and may differ from `time` for efficiency.

Invoking this method with positiveInfinity for `toleranceBefore` and `toleranceAfter` is the same as invoking seek(to:completionHandler:) directly.

Seeking is constrained by the collection of seekable time ranges. If you seek to a time outside all of the seekable ranges, the seek will result in a current time within the seekable ranges.

## See Also

### Seeking Through Media

func seek(to: CMTime, completionHandler: ((Bool) -> Void)?)

Sets the current playback time to the specified time.

func seek(to: Date, completionHandler: ((Bool) -> Void)?) -> Bool

Sets the current playback time to the time specified by the date object.

func cancelPendingSeeks()

Cancels any pending seek requests and invokes the corresponding completion handlers if present.

