

- AVFoundation
- AVPlayerItem
-  cancelPendingSeeks() 

Instance Method

# cancelPendingSeeks()

Cancels any pending seek requests and invokes the corresponding completion handlers if present.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func cancelPendingSeeks()
```

## Discussion

Use this method to cancel and release the completion handlers of pending seeks.

The `finished` parameter of the completion handlers will be set to false.

## See Also

### Seeking Through Media

func seek(to: CMTime, completionHandler: ((Bool) -> Void)?)

Sets the current playback time to the specified time.

func seek(to: CMTime, toleranceBefore: CMTime, toleranceAfter: CMTime, completionHandler: ((Bool) -> Void)?)

Sets the current playback time within a specified time bound and invokes the specified block when the seek operation completes or is interrupted.

func seek(to: Date, completionHandler: ((Bool) -> Void)?) -> Bool

Sets the current playback time to the time specified by the date object.

