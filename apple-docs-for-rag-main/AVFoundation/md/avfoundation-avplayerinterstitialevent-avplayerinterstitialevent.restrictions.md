

- AVFoundation
- AVPlayerInterstitialEvent
-  AVPlayerInterstitialEvent.Restrictions 

Structure

# AVPlayerInterstitialEvent.Restrictions

Constants that define restrictions on the playback of interstitial content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Restrictions
```

## Topics

### Configure

static var constrainsSeekingForwardInPrimaryContent: AVPlayerInterstitialEvent.Restrictions

A restriction that indicates the event doesn’t allow seeking forward within an interstitial item.

static var requiresPlaybackAtPreferredRateForAdvancement: AVPlayerInterstitialEvent.Restrictions

A restriction that indicates the event doesn’t allow advancing the current time within an interstitial item.

### Initializing a Restriction

init(rawValue: UInt)

Creates a restriction with an integer.

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

### Managing restrictions

var restrictions: AVPlayerInterstitialEvent.Restrictions

The restrictions the event imposes on the playback of interstitial content.

