

- AVFoundation
- AVPlayerInterstitialEvent
-  primaryItem 

Instance Property

# primaryItem

The player item that represents the primary content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
weak var primaryItem: AVPlayerItem? { get }
```

## Discussion

The item must contain an AVAsset that provides intrinsic mappings from its timeline to realtime dates.

## See Also

### Accessing player items

var templateItems: [AVPlayerItem]

An array of player item configurations to use as templates for player items that play interstitial content.

