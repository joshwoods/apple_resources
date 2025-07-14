

- AVFoundation
- AVPartialAsyncProperty
-  availableMetadataFormats 

Type Property

# availableMetadataFormats

The formats of metadata that an asset contains.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var availableMetadataFormats: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Mentioned in 

Retrieving media metadata

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for all metadata identifiers.

static var commonMetadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for common metadata identifiers.

func loadMetadata(for: AVMetadataFormat, completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads an array of metadata items that the asset contains for the specified format.

static var creationDate: AVAsyncProperty&lt;Root, AVMetadataItem?>

A metadata item that indicates the creation date of an asset.

static var lyrics: AVAsyncProperty&lt;Root, String?>

The lyrics of the asset in a language suitable for the current locale.

