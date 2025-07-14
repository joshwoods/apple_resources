

- PHASE
- PHASESoundAsset
-  url 

Instance Property

# url

The URL of the sound asset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var url: URL? { get }
```

## Discussion

This property has a value when an app creates the asset with registerSoundAsset(url:identifier:assetType:channelLayout:normalizationMode:); otherwise the value is `nil`.

## See Also

### Accessing Sound Data

var data: Data?

A storage buffer for the sound asset.

