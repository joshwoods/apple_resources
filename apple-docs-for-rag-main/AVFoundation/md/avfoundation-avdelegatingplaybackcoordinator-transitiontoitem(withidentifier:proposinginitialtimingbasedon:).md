

- AVFoundation
- AVDelegatingPlaybackCoordinator
-  transitionToItem(withIdentifier:proposingInitialTimingBasedOn:) 

Instance Method

# transitionToItem(withIdentifier:proposingInitialTimingBasedOn:)

Tells the coordinator to transition to a new item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func transitionToItem(
    withIdentifier itemIdentifier: String?,
    proposingInitialTimingBasedOn snapshotTimebase: CMTimebase?
)
```

## Parameters 

`itemIdentifier`  

The identifier for the new current item, which is `nil` if there isn’t anything to play.

`snapshotTimebase`  

A time base that communicates the initial playback state of the new item. If you specify `nil`, the coordinator assumes that the player pauses at zero.

You can retrieve an appropriate time base to pass for this value from AVFoundation playback objects like AVSampleBufferRenderSynchronizer. You can also create one manually using the CMTimebaseCreateWithSourceClock(allocator:sourceClock:timebaseOut:) function.

## See Also

### Coordinating State Changes

func coordinateRateChange(to: Float, options: AVDelegatingPlaybackCoordinatorRateChangeOptions)

Coordinates a rate change across all participants, waiting for others to become ready, if necessary.

func coordinateSeek(to: CMTime, options: AVDelegatingPlaybackCoordinatorSeekOptions)

Coordinates a seek to the specified time for all connected participants.

func reapplyCurrentItemStateToPlaybackControlDelegate()

Tells the coordinator to reissue current play state commands to synchronize the current item to the state of other participants.

struct AVDelegatingPlaybackCoordinatorSeekOptions

Constants that define seek options.

struct AVDelegatingPlaybackCoordinatorRateChangeOptions

Constants that define rate change options.

