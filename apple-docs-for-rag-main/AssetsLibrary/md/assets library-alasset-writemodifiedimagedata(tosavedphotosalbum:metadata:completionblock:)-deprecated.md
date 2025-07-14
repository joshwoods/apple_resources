

- Assets Library
- ALAsset
-  writeModifiedImageData(toSavedPhotosAlbum:metadata:completionBlock:) Deprecated

Instance Method

# writeModifiedImageData(toSavedPhotosAlbum:metadata:completionBlock:)

Saves image data to the Saved Photos album.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**iOS, iPadOS, Mac Catalyst**

``` source
func writeModifiedImageData(
    toSavedPhotosAlbum imageData: Data!,
    metadata: [AnyHashable : Any]!,
    completionBlock: ALAssetsLibraryWriteImageCompletionBlock!
)
```

**Mac Catalyst**

``` source
func writeModifiedImageData(
    toSavedPhotosAlbum imageData: Data!,
    metadata: [AnyHashable : Any]!
) async throws -> URL?
```

Deprecated

Use creationRequestForAssetFromImage: on PHAssetChangeRequest from the Photos framework to create a new asset instead

## Parameters 

`imageData`  

Image data for the asset.

`metadata`  

Metadata for the image.

`completionBlock`  

The block invoked after the save operation completes.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeModifiedImageData(toSavedPhotosAlbum imageData: Data!, metadata: [AnyHashable : Any]!) async throws -> URL?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method saves `imageData` to the saved photos album as a new asset that is considered a modified version of the receiver.

## See Also

### Saving to the Saved Photos Album

func writeModifiedVideoAtPath(toSavedPhotosAlbum: URL!, completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!)

Saves the video at a specified path to the Saved Photos album.

Deprecated

