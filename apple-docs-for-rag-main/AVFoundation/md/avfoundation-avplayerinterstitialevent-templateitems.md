

- AVFoundation
- AVPlayerInterstitialEvent
-  templateItems 

Instance Property

# templateItems

An array of player item configurations to use as templates for player items that play interstitial content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var templateItems: [AVPlayerItem] { get set }
```

## Discussion

If you require the system to create new player items using the same asset instance as the template item, create the asset with an AVURLAssetPrimarySessionIdentifierKey value equal to httpSessionIdentifier of the primary item’s asset. Creating assets this way simplifies cases where you require loading their data with a custom AVAssetResourceLoader delegate.

Important

The system raises an exception if template items contain assets that aren’t URL based, such as AVComposition.

## See Also

### Accessing player items

var primaryItem: AVPlayerItem?

The player item that represents the primary content.

