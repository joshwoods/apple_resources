

- AVFoundation
- AVDelegatingPlaybackCoordinator
-  reapplyCurrentItemStateToPlaybackControlDelegate() 

Instance Method

# reapplyCurrentItemStateToPlaybackControlDelegate()

Tells the coordinator to reissue current play state commands to synchronize the current item to the state of other participants.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func reapplyCurrentItemStateToPlaybackControlDelegate()
```

## See Also

### Coordinating State Changes

func coordinateRateChange(to: Float, options: AVDelegatingPlaybackCoordinatorRateChangeOptions)

Coordinates a rate change across all participants, waiting for others to become ready, if necessary.

func coordinateSeek(to: CMTime, options: AVDelegatingPlaybackCoordinatorSeekOptions)

Coordinates a seek to the specified time for all connected participants.

func transitionToItem(withIdentifier: String?, proposingInitialTimingBasedOn: CMTimebase?)

Tells the coordinator to transition to a new item.

struct AVDelegatingPlaybackCoordinatorSeekOptions

Constants that define seek options.

struct AVDelegatingPlaybackCoordinatorRateChangeOptions

Constants that define rate change options.

