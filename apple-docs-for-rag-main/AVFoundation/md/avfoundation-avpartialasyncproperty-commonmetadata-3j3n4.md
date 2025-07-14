

- AVFoundation
- AVPartialAsyncProperty
-  commonMetadata 

Type Property

# commonMetadata

The metadata items that an asset contains for common metadata identifiers.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var commonMetadata: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Mentioned in 

Retrieving media metadata

## Discussion

Use the load(_:) method to retrieve the property value.

The value contains an array of metadata items that contain an identifier value from the set of Common Metadata Identifiers.

You can filter items in this array according to language by calling metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:), or by identifier by calling metadataItems(from:filteredByIdentifier:).

## See Also

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for all metadata identifiers.

static var availableMetadataFormats: AVAsyncProperty&lt;Root, [AVMetadataFormat]>

The formats of metadata that an asset contains.

func loadMetadata(for: AVMetadataFormat, completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads an array of metadata items that the asset contains for the specified format.

static var creationDate: AVAsyncProperty&lt;Root, AVMetadataItem?>

A metadata item that indicates the creation date of an asset.

static var lyrics: AVAsyncProperty&lt;Root, String?>

The lyrics of the asset in a language suitable for the current locale.

