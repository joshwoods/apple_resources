

- AVFoundation
- AVDelegatingPlaybackCoordinator
-  coordinateSeek(to:options:) 

Instance Method

# coordinateSeek(to:options:)

Coordinates a seek to the specified time for all connected participants.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func coordinateSeek(
    to time: CMTime,
    options: AVDelegatingPlaybackCoordinatorSeekOptions = []
)
```

## Parameters 

`time`  

A time the group seeks to when the command ends.

`options`  

Additional configuration of the seek.

## Discussion

To end a suspension and also affect the group timing, see end(proposingNewTime:).

Note

Calling this method while the coordinator is in a suspended state affects only the local playback object. It doesn’t affect group state, even after the suspension ends.

## See Also

### Coordinating State Changes

func coordinateRateChange(to: Float, options: AVDelegatingPlaybackCoordinatorRateChangeOptions)

Coordinates a rate change across all participants, waiting for others to become ready, if necessary.

func transitionToItem(withIdentifier: String?, proposingInitialTimingBasedOn: CMTimebase?)

Tells the coordinator to transition to a new item.

func reapplyCurrentItemStateToPlaybackControlDelegate()

Tells the coordinator to reissue current play state commands to synchronize the current item to the state of other participants.

struct AVDelegatingPlaybackCoordinatorSeekOptions

Constants that define seek options.

struct AVDelegatingPlaybackCoordinatorRateChangeOptions

Constants that define rate change options.

