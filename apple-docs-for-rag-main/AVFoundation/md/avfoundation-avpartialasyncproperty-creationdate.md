

- AVFoundation
- AVPartialAsyncProperty
-  creationDate 

Type Property

# creationDate

A metadata item that indicates the creation date of an asset.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var creationDate: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

If the asset stores a creation date in a form the system can convert to an NSDate, the metadata item’s dateValue property contains a valid date. Otherwise, the creation date is available only as a string that you retrieve by calling the metadata item’s stringValue property.

This property may be `nil`.

## See Also

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for all metadata identifiers.

static var commonMetadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for common metadata identifiers.

static var availableMetadataFormats: AVAsyncProperty&lt;Root, [AVMetadataFormat]>

The formats of metadata that an asset contains.

func loadMetadata(for: AVMetadataFormat, completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads an array of metadata items that the asset contains for the specified format.

static var lyrics: AVAsyncProperty&lt;Root, String?>

The lyrics of the asset in a language suitable for the current locale.

