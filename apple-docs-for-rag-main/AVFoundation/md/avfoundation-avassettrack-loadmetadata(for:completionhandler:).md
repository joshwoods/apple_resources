

- AVFoundation
- AVAssetTrack
-  loadMetadata(for:completionHandler:) 

Instance Method

# loadMetadata(for:completionHandler:)

Loads metadata items that a track contains for the specified format.

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
The loaded metadata, or an empty array if no metadata items for the specified format exist. The value is `nil` if an error occurs.

error  
An error object if the request fails; otherwise, nil.

## See Also

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

An array of metadata items for all metadata identifiers that have a value.

static var commonMetadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

An array of metadata items for all common metadata keys that have a value.

static var availableMetadataFormats: AVAsyncProperty&lt;Root, [AVMetadataFormat]>

An array of metadata formats available for the track.

