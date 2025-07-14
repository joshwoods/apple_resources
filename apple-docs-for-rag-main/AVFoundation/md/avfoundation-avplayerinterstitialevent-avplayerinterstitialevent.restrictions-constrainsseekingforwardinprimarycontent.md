

- AVFoundation
- AVPlayerInterstitialEvent
- AVPlayerInterstitialEvent.Restrictions
-  constrainsSeekingForwardInPrimaryContent 

Type Property

# constrainsSeekingForwardInPrimaryContent

A restriction that indicates the event doesn’t allow seeking forward within an interstitial item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var constrainsSeekingForwardInPrimaryContent: AVPlayerInterstitialEvent.Restrictions { get }
```

## See Also

### Configure

static var requiresPlaybackAtPreferredRateForAdvancement: AVPlayerInterstitialEvent.Restrictions

A restriction that indicates the event doesn’t allow advancing the current time within an interstitial item.

