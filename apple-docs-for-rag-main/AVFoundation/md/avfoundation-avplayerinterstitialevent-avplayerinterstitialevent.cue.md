

- AVFoundation
- AVPlayerInterstitialEvent
-  AVPlayerInterstitialEvent.Cue 

Structure

# AVPlayerInterstitialEvent.Cue

A structure that defines standard cues to play interstitial content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Cue
```

## Topics

### Cues

static let noCue: AVPlayerInterstitialEvent.Cue

A cue that indicates that playback starts at the interstitial event time or date.

static let joinCue: AVPlayerInterstitialEvent.Cue

A cue that indicates that playback occurs before starting primary playback, regardless of initial primary playback position.

static let leaveCue: AVPlayerInterstitialEvent.Cue

A cue that indicates event playback occurs after primary playback ends without error, either at the end of the primary asset or at the client-specified forward playback end time.

### Initializers

init(rawValue: String)

Creates an interstitial event cue from its raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring cues

var cue: AVPlayerInterstitialEvent.Cue

A cue to schedule interstitial event playback at a predefined position during primary playback.

