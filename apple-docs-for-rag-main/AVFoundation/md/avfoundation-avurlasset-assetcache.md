

- AVFoundation
- AVURLAsset
-  assetCache 

Instance Property

# assetCache

The asset’s associated asset cache, if it exists.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var assetCache: AVAssetCache? { get }
```

## Discussion

This property provides access to an instance of AVAssetCache to use for inspection of locally cached media data. The value of this property is `nil` if you haven’t configured the asset to store or access media data from disk.

