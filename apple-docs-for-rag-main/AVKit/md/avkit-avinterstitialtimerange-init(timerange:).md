

- AVKit
- AVInterstitialTimeRange
-  init(timeRange:) 

Initializer

# init(timeRange:)

Initializes an interstitial time range object with the specified time range.

tvOS 9.0+

``` source
init(timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

The time range to designate as interstitial content.

## Return Value

A new interstitial time range object.

## Discussion

To associate interstitial time ranges with an asset for playback, use the interstitialTimeRanges property of an AVPlayerItem object.

