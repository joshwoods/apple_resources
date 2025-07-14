

- Assets Library
- ALAssetsLibrary
-  writeImageData(toSavedPhotosAlbum:metadata:completionBlock:) Deprecated

Instance Method

# writeImageData(toSavedPhotosAlbum:metadata:completionBlock:)

Writes given image data and metadata to the Photos Album.

iOS 4.1–9.0DeprecatediPadOS 4.1–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**iOS, iPadOS, Mac Catalyst**

``` source
func writeImageData(
    toSavedPhotosAlbum imageData: Data!,
    metadata: [AnyHashable : Any]!,
    completionBlock: ALAssetsLibraryWriteImageCompletionBlock!
)
```

**Mac Catalyst**

``` source
func writeImageData(
    toSavedPhotosAlbum imageData: Data!,
    metadata: [AnyHashable : Any]!
) async throws -> URL?
```

Deprecated

Use creationRequestForAssetFromImageData: on PHAssetChangeRequest from the Photos framework to create a new asset instead

## Parameters 

`imageData`  

Data for the image to add to the album.

`metadata`  

The metadata to associate with the image.

`completionBlock`  

The block invoked after the save operation completes.

For a description of the block, see ALAssetsLibraryWriteImageCompletionBlock.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeImageData(toSavedPhotosAlbum imageData: Data!, metadata: [AnyHashable : Any]!) async throws -> URL?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If there is a conflict between the metadata in the image data and the metadata dictionary, the image data metadata values will be overwritten.

## See Also

### Saving Assets

func writeVideoAtPath(toSavedPhotosAlbum: URL!, completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!)

Saves a video identified by a given URL to the Saved Photos album.

Deprecated

func videoAtPathIs(compatibleWithSavedPhotosAlbum: URL!) -> Bool

Returns a Boolean value that indicates whether a video identified by a given URL is compatible with the Saved Photos album.

Deprecated

func writeImage(toSavedPhotosAlbum: CGImage!, orientation: ALAssetOrientation, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Saves a given image to the Saved Photos album.

Deprecated

func writeImage(toSavedPhotosAlbum: CGImage!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Writes a given image and metadata to the Photos Album.

Deprecated

