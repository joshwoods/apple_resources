

- Assets Library
- ALAssetsLibrary
-  writeImage(toSavedPhotosAlbum:orientation:completionBlock:) Deprecated

Instance Method

# writeImage(toSavedPhotosAlbum:orientation:completionBlock:)

Saves a given image to the Saved Photos album.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**iOS, iPadOS, Mac Catalyst**

``` source
func writeImage(
    toSavedPhotosAlbum imageRef: CGImage!,
    orientation: ALAssetOrientation,
    completionBlock: ALAssetsLibraryWriteImageCompletionBlock!
)
```

**Mac Catalyst**

``` source
func writeImage(
    toSavedPhotosAlbum imageRef: CGImage!,
    orientation: ALAssetOrientation
) async throws -> URL?
```

Deprecated

Use creationRequestForAssetFromImage: on PHAssetChangeRequest from the Photos framework to create a new asset instead

## Parameters 

`imageRef`  

The image to save to the Saved Photos album.

`orientation`  

The orientation at which to save the image.

`completionBlock`  

The block invoked after the save operation completes.

For a description of the block, see ALAssetsLibraryWriteImageCompletionBlock.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeImage(toSavedPhotosAlbum imageRef: CGImage!, orientation: ALAssetOrientation) async throws -> URL?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If you want to save a UIImage object, you can use the `UIImage` method CGImage to get a `CGImageRef`, and cast the image’s imageOrientation to `ALAssetOrientation`.

## See Also

### Saving Assets

func writeVideoAtPath(toSavedPhotosAlbum: URL!, completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!)

Saves a video identified by a given URL to the Saved Photos album.

Deprecated

func videoAtPathIs(compatibleWithSavedPhotosAlbum: URL!) -> Bool

Returns a Boolean value that indicates whether a video identified by a given URL is compatible with the Saved Photos album.

Deprecated

func writeImageData(toSavedPhotosAlbum: Data!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Writes given image data and metadata to the Photos Album.

Deprecated

func writeImage(toSavedPhotosAlbum: CGImage!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Writes a given image and metadata to the Photos Album.

Deprecated

