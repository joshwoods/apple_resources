

- AVFoundation
- AVPlayerItem
-  automaticallyHandlesInterstitialEvents 

Instance Property

# automaticallyHandlesInterstitialEvents

A Boolean value that indicates whether the player item automatically plays interstitial events according to server-side directives.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
var automaticallyHandlesInterstitialEvents: Bool { get set }
```

## See Also

### Configuring Interstitial Events

var integratedTimeline: AVPlayerItemIntegratedTimeline

An integrated timeline that represents the player item timing including its scheduled interstitial events.

var translatesPlayerInterstitialEvents: Bool

A Boolean value that indicates whether the player translates interstitial events to interstitial time ranges.

var interstitialTimeRanges: [AVInterstitialTimeRange]

An array of time ranges that identify interstitial content.

var template: AVPlayerItem?

The template player item that initializes this instance.

