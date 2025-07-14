

- Assets Library
- ALAssetsLibrary
-  writeVideoAtPath(toSavedPhotosAlbum:completionBlock:) Deprecated

Instance Method

# writeVideoAtPath(toSavedPhotosAlbum:completionBlock:)

Saves a video identified by a given URL to the Saved Photos album.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**iOS, iPadOS, Mac Catalyst**

``` source
func writeVideoAtPath(
    toSavedPhotosAlbum videoPathURL: URL!,
    completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!
)
```

**Mac Catalyst**

``` source
func writeVideoAtPath(toSavedPhotosAlbum videoPathURL: URL!) async throws -> URL?
```

Deprecated

Use creationRequestForAssetFromVideoAtFilePath: on PHAssetChangeRequest from the Photos framework to create a new asset instead

## Parameters 

`videoPathURL`  

An URL that points to a video file.

`completionBlock`  

The block invoked after the save operation completes.

For a description of the block, see ALAssetsLibraryWriteVideoCompletionBlock.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeVideoAtPath(toSavedPhotosAlbum videoPathURL: URL!) async throws -> URL?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Saving Assets

func videoAtPathIs(compatibleWithSavedPhotosAlbum: URL!) -> Bool

Returns a Boolean value that indicates whether a video identified by a given URL is compatible with the Saved Photos album.

Deprecated

func writeImage(toSavedPhotosAlbum: CGImage!, orientation: ALAssetOrientation, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Saves a given image to the Saved Photos album.

Deprecated

func writeImageData(toSavedPhotosAlbum: Data!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Writes given image data and metadata to the Photos Album.

Deprecated

func writeImage(toSavedPhotosAlbum: CGImage!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Writes a given image and metadata to the Photos Album.

Deprecated

