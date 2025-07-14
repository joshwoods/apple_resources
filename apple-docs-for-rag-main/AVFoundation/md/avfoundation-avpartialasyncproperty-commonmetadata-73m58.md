

- AVFoundation
- AVPartialAsyncProperty
-  commonMetadata 

Type Property

# commonMetadata

An array of metadata items for all common metadata keys that have a value.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var commonMetadata: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

You can filter the array of metadata items according to language using the metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:) method. Filter the results by identifier using the metadataItems(from:filteredByIdentifier:) method.

## See Also

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

An array of metadata items for all metadata identifiers that have a value.

static var availableMetadataFormats: AVAsyncProperty&lt;Root, [AVMetadataFormat]>

An array of metadata formats available for the track.

func loadMetadata(for: AVMetadataFormat, completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads metadata items that a track contains for the specified format.

