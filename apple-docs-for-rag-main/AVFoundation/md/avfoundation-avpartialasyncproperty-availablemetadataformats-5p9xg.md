

- AVFoundation
- AVPartialAsyncProperty
-  availableMetadataFormats 

Type Property

# availableMetadataFormats

An array of metadata formats available for the track.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var availableMetadataFormats: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

An array of metadata items for all metadata identifiers that have a value.

static var commonMetadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

An array of metadata items for all common metadata keys that have a value.

func loadMetadata(for: AVMetadataFormat, completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads metadata items that a track contains for the specified format.

