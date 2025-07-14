

- AVFoundation
- AVComposition
-  metadata 

Instance Property

# metadata

An array of metadata items for all metadata identifiers for which a value is available.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var metadata: [AVMetadataItem] { get }
```

## Discussion

You can filter the metadata items by language using the metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:) method, or by identifier with the metadataItems(from:filteredByIdentifier:) method.

## See Also

### Accessing Metadata

var commonMetadata: [AVMetadataItem]

The metadata items an asset contains for common metadata identifiers that provide a value.

var availableMetadataFormats: [AVMetadataFormat]

The metadata formats this asset contains.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns an array of metadata items from the container with the specified format.

var creationDate: AVMetadataItem?

A metadata item that indicates the asset’s creation date.

var lyrics: String?

The lyrics of the asset in a language suitable for the current locale.

