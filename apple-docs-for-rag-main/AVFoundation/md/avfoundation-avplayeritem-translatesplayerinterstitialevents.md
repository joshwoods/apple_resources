

- AVFoundation
- AVPlayerItem
-  translatesPlayerInterstitialEvents 

Instance Property

# translatesPlayerInterstitialEvents

A Boolean value that indicates whether the player translates interstitial events to interstitial time ranges.

tvOS 15.0+

``` source
@MainActor
var translatesPlayerInterstitialEvents: Bool { get set }
```

## Discussion

Enable this property value to support using interstitial events, or set it to false to perform your own interstitial management.

## See Also

### Configuring Interstitial Events

var integratedTimeline: AVPlayerItemIntegratedTimeline

An integrated timeline that represents the player item timing including its scheduled interstitial events.

var automaticallyHandlesInterstitialEvents: Bool

A Boolean value that indicates whether the player item automatically plays interstitial events according to server-side directives.

var interstitialTimeRanges: [AVInterstitialTimeRange]

An array of time ranges that identify interstitial content.

var template: AVPlayerItem?

The template player item that initializes this instance.

