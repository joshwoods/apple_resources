

- AVFoundation
- AVMutableMovie
-  metadata(forFormat:) 

Instance Method

# metadata(forFormat:)

Returns an array of metadata items from the container with the specified format.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func metadata(forFormat format: AVMetadataFormat) -> [AVMetadataItem]
```

## Parameters 

`format`  

The metadata format for which you want items.

## Return Value

An array of AVMetadataItem objects, one for each metadata item in the container of the specified format, or an empty array if there is no metadata for the specified format.

## Discussion

You can filter the array to the specific items of interest using the class methods provided by AVMetadataItem, like metadataItems(from:filteredByIdentifier:) or metadataItems(from:with:).

You can call this method without blocking the current thread after you’ve asynchronously loaded the availableMetadataFormats property.

## See Also

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers for which a value is available.

var commonMetadata: [AVMetadataItem]

The metadata items an asset contains for common metadata identifiers that provide a value.

var availableMetadataFormats: [AVMetadataFormat]

The metadata formats this asset contains.

var creationDate: AVMetadataItem?

A metadata item that indicates the asset’s creation date.

var lyrics: String?

The lyrics of the asset in a language suitable for the current locale.

