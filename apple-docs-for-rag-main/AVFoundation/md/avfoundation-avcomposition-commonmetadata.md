

- AVFoundation
- AVComposition
-  commonMetadata 

Instance Property

# commonMetadata

The metadata items an asset contains for common metadata identifiers that provide a value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var commonMetadata: [AVMetadataItem] { get }
```

## Discussion

This property value is an array of metadata items, one for each metadata key from the common key space for which the asset has an available value. You can use the various class methods provided by AVMetadataItem, such as metadataItems(from:filteredByIdentifier:) or metadataItems(from:with:) to filter the array to the specific items of interest.

## See Also

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers for which a value is available.

var availableMetadataFormats: [AVMetadataFormat]

The metadata formats this asset contains.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns an array of metadata items from the container with the specified format.

var creationDate: AVMetadataItem?

A metadata item that indicates the asset’s creation date.

var lyrics: String?

The lyrics of the asset in a language suitable for the current locale.

