

- AVFoundation
- AVCompositionTrack
-  metadata 

Instance Property

# metadata

An array of metadata items for all metadata identifiers that have a value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var metadata: [AVMetadataItem] { get }
```

## Discussion

You can filter the array of metadata items according to language using the metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:) method. Filter the results by identifier using the metadataItems(from:filteredByIdentifier:) method.

## See Also

### Accessing Metadata

var commonMetadata: [AVMetadataItem]

An array of metadata items for all common metadata keys that have a value.

var availableMetadataFormats: [AVMetadataFormat]

An array of metadata formats available for the track.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns metadata items that a track contains for the specified format.

