

- AVFoundation
- AVComposition
-  creationDate 

Instance Property

# creationDate

A metadata item that indicates the asset’s creation date.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var creationDate: AVMetadataItem? { get }
```

## Discussion

If the asset contains metadata that the framework can convert to an NSDate, you can retrieve it from the metadata item using its dateValue property. Otherwise, you retrieve it as a string by using the metadata item’s stringValue property.

This property value is `nil` if no creation date metadata exists.

## See Also

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers for which a value is available.

var commonMetadata: [AVMetadataItem]

The metadata items an asset contains for common metadata identifiers that provide a value.

var availableMetadataFormats: [AVMetadataFormat]

The metadata formats this asset contains.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns an array of metadata items from the container with the specified format.

var lyrics: String?

The lyrics of the asset in a language suitable for the current locale.

