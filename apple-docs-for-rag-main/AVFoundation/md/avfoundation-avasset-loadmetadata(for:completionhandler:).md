

- AVFoundation
- AVAsset
-  loadMetadata(for:completionHandler:) 

Instance Method

# loadMetadata(for:completionHandler:)

Loads an array of metadata items that the asset contains for the specified format.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadMetadata(
    for format: AVMetadataFormat,
    completionHandler: @escaping ([AVMetadataItem]?, (any Error)?) -> Void
)
```

``` source
func loadMetadata(for format: AVMetadataFormat) async throws -> [AVMetadataItem]
```

## Parameters 

`format`  

The format of the metadata items to load.

`completionHandler`  

A callback that the system invokes after it finishes the loading request. It passes the completion handler the following parameters:

metadata  
An array of metadata items, which may be empty if there are no items of the specified format. The value is `nil` if an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## Mentioned in 

Retrieving media metadata

## See Also

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for all metadata identifiers.

static var commonMetadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for common metadata identifiers.

static var availableMetadataFormats: AVAsyncProperty&lt;Root, [AVMetadataFormat]>

The formats of metadata that an asset contains.

static var creationDate: AVAsyncProperty&lt;Root, AVMetadataItem?>

A metadata item that indicates the creation date of an asset.

static var lyrics: AVAsyncProperty&lt;Root, String?>

The lyrics of the asset in a language suitable for the current locale.

