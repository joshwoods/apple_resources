

- AVFoundation
- AVPlayerItem
-  interstitialTimeRanges 

Instance Property

# interstitialTimeRanges

An array of time ranges that identify interstitial content.

iOS 16.0+iPadOS 16.0+tvOSvisionOS 1.0+

**iOS, iPadOS, visionOS**

``` source
@MainActor
var interstitialTimeRanges: [AVInterstitialTimeRange] { get }
```

**tvOS**

``` source
@MainActor
var interstitialTimeRanges: [AVInterstitialTimeRange] { get set }
```

## Discussion

Interstitial content is material that’s unrelated to a player item’s primary content, such as advertisements and legal notices. If you use AVPlayerViewController to present an item that contains interstitial time ranges, the user interface marks those time ranges differently on the playback timeline. A player view controller can also call your app when it begins and ends playing interstitial content. You can use these events to customize playback behavior, such as preventing viewers from skipping required content.

Note

On iOS, the stream must define the interstitial time ranges, or you must use AVPlayerInterstitialEventController.

## See Also

### Configuring Interstitial Events

var integratedTimeline: AVPlayerItemIntegratedTimeline

An integrated timeline that represents the player item timing including its scheduled interstitial events.

var automaticallyHandlesInterstitialEvents: Bool

A Boolean value that indicates whether the player item automatically plays interstitial events according to server-side directives.

var translatesPlayerInterstitialEvents: Bool

A Boolean value that indicates whether the player translates interstitial events to interstitial time ranges.

var template: AVPlayerItem?

The template player item that initializes this instance.

