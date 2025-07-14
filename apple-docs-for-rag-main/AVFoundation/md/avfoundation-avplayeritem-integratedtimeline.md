

- AVFoundation
- AVPlayerItem
-  integratedTimeline 

Instance Property

# integratedTimeline

An integrated timeline that represents the player item timing including its scheduled interstitial events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
var integratedTimeline: AVPlayerItemIntegratedTimeline { get }
```

## Discussion

The value is `nil` for player items in an interstitial player.

## See Also

### Configuring Interstitial Events

var automaticallyHandlesInterstitialEvents: Bool

A Boolean value that indicates whether the player item automatically plays interstitial events according to server-side directives.

var translatesPlayerInterstitialEvents: Bool

A Boolean value that indicates whether the player translates interstitial events to interstitial time ranges.

var interstitialTimeRanges: [AVInterstitialTimeRange]

An array of time ranges that identify interstitial content.

var template: AVPlayerItem?

The template player item that initializes this instance.

