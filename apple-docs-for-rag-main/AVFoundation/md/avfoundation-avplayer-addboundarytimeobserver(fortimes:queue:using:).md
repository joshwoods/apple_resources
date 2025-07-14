

- AVFoundation
- AVPlayer
-  addBoundaryTimeObserver(forTimes:queue:using:) 

Instance Method

# addBoundaryTimeObserver(forTimes:queue:using:)

Requests the invocation of a block when specified times are traversed during normal playback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func addBoundaryTimeObserver(
    forTimes times: [NSValue],
    queue: dispatch_queue_t?,
    using block: @escaping () -> Void
) -> Any
```

## Parameters 

`times`  

An array of `NSValue` objects containing CMTime values that represent the times at which to invoke the callback. The system raises an exception if you pass an empty array.

`queue`  

A *serial* queue onto which `block` should be enqueued. Passing a concurrent queue is not supported and will result in undefined behavior.

If you pass `nil`, the main queue is used.

`block`  

The block to be invoked when any of the times in `times` is crossed during normal playback.

## Return Value

An opaque object that you pass as the argument to removeTimeObserver(_:) to stop observation.

## Mentioned in 

Monitoring playback progress in your app

## Discussion

Boundary times are arbitrary points of interest you define within the media timeline. As these times are traversed during normal playback, the block you provide to this method will be invoked. You must maintain a strong reference to the returned value as long as you want the time observer to be invoked by the player. Each invocation of this method should be paired with a corresponding call to removeTimeObserver(_:).

The player does not guarantee the callback block will always be invoked for each boundary time. If your times are very close together along the timeline (close enough that the execution of the block for one takes longer than the difference between them) or if a seek causes time to jump over one or more boundary times, time observation for any specific boundary time may not occur. The best practice is therefore to implement the callback block so it always performs its necessary calculations based solely on the player’s currentTime().

The following example shows how you could define boundary times for each quarter of playback.

- Swift
- Objective-C

```
func addBoundaryTimeObserver() {
    var times = [NSValue]()
    // Set initial time to zero
    var currentTime = CMTime.zero
    // Divide the asset's duration into quarters.
    let interval = CMTimeMultiplyByFloat64(asset.duration, multiplier: 0.25)

    // Build boundary times at 25%, 50%, 75%, 100%
    while currentTime 

```
- (void)addBoundaryTimeObserver {
    NSMutableArray *times = [NSMutableArray array];

    // Set initial time to zero
    CMTime currentTime = kCMTimeZero;
    // Get asset duration
    CMTime assetDuration = self.asset.duration;
    // Divide the asset duration into quarters
    CMTime interval = CMTimeMultiplyByFloat64(assetDuration, 0.25);

    // Build boundary times at 25%, 50%, 75%, 100%
    while (CMTIME_COMPARE_INLINE(currentTime, 

Important

Use a `weak` reference to `self` in the callback block to prevent creating a retain cycle.

## See Also

### Observing Playback Time

func currentTime() -> CMTime

Returns the current time of the current player item.

func addPeriodicTimeObserver(forInterval: CMTime, queue: dispatch_queue_t?, using: (CMTime) -> Void) -> Any

Requests the periodic invocation of a given block during playback to report changing time.

func removeTimeObserver(Any)

Cancels a previously registered periodic or boundary time observer.

