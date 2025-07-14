

- AVFoundation
- AVComposition
-  availableMetadataFormats 

Instance Property

# availableMetadataFormats

The metadata formats this asset contains.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var availableMetadataFormats: [AVMetadataFormat] { get }
```

## Discussion

Metadata formats may include ID3, iTunes metadata, and so on.

## See Also

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers for which a value is available.

var commonMetadata: [AVMetadataItem]

The metadata items an asset contains for common metadata identifiers that provide a value.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns an array of metadata items from the container with the specified format.

var creationDate: AVMetadataItem?

A metadata item that indicates the asset’s creation date.

var lyrics: String?

The lyrics of the asset in a language suitable for the current locale.

