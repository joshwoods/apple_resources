

- PHASE
- PHASESoundAsset
-  data 

Instance Property

# data

A storage buffer for the sound asset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var data: Data? { get }
```

## Discussion

This property has a value when an app creates the asset with registerSoundAsset(data:identifier:format:normalizationMode:); otherwise the value is `nil`.

## See Also

### Accessing Sound Data

var url: URL?

The URL of the sound asset.

