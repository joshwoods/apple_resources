

- AVFoundation
- AVPlayerItem
-  seek(to:completionHandler:) 

Instance Method

# seek(to:completionHandler:)

Sets the current playback time to the specified time.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func seek(
    to time: CMTime,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
nonisolated
func seek(to time: CMTime) async -> Bool
```

## Parameters 

`time`  

The time to which to seek.

`completionHandler`  

The block to invoke when the seek operation has either been completed or been interrupted. The block takes one argument:

finished  
Indicates whether the seek operation completed.

## Discussion

Use this method to seek to a specified time in the player item and be notified when the operation completes. If the seek request completes without being interrupted (either by another seek request or by any other operation), the completion handler you provide is executed with the `finished` parameter set to true.

If another seek request is already in progress when you call this method, the completion handler for the in-progress seek request is executed immediately with the `finished` parameter set to false.

## See Also

### Seeking Through Media

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: ((Bool) -> Void)?)

Sets the current playback time within a specified time bound and invokes the specified block when the seek operation completes or is interrupted.

func seek(to: Date, completionHandler: ((Bool) -> Void)?) -> Bool

Sets the current playback time to the time specified by the date object.

func cancelPendingSeeks()

Cancels any pending seek requests and invokes the corresponding completion handlers if present.

