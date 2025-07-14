

- AVFoundation
-  AVDelegatingPlaybackCoordinatorSeekOptions 

Structure

# AVDelegatingPlaybackCoordinatorSeekOptions

Constants that define seek options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct AVDelegatingPlaybackCoordinatorSeekOptions
```

## Topics

### Seek Options

static var resumeImmediately: AVDelegatingPlaybackCoordinatorSeekOptions

An option that Indicates that the coordinator needs to resume playback as soon as possible, regardless of other participant’s readiness or suspensions.

### Initializers

init(rawValue: UInt)

Creates a rate change option with a string.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Coordinating State Changes

func coordinateRateChange(to: Float, options: AVDelegatingPlaybackCoordinatorRateChangeOptions)

Coordinates a rate change across all participants, waiting for others to become ready, if necessary.

func coordinateSeek(to: CMTime, options: AVDelegatingPlaybackCoordinatorSeekOptions)

Coordinates a seek to the specified time for all connected participants.

func transitionToItem(withIdentifier: String?, proposingInitialTimingBasedOn: CMTimebase?)

Tells the coordinator to transition to a new item.

func reapplyCurrentItemStateToPlaybackControlDelegate()

Tells the coordinator to reissue current play state commands to synchronize the current item to the state of other participants.

struct AVDelegatingPlaybackCoordinatorRateChangeOptions

Constants that define rate change options.

