

- Assets Library
- ALAsset
-  writeModifiedVideoAtPath(toSavedPhotosAlbum:completionBlock:) Deprecated

Instance Method

# writeModifiedVideoAtPath(toSavedPhotosAlbum:completionBlock:)

Saves the video at a specified path to the Saved Photos album.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**iOS, iPadOS, Mac Catalyst**

``` source
func writeModifiedVideoAtPath(
    toSavedPhotosAlbum videoPathURL: URL!,
    completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!
)
```

**Mac Catalyst**

``` source
func writeModifiedVideoAtPath(toSavedPhotosAlbum videoPathURL: URL!) async throws -> URL?
```

Deprecated

Use creationRequestForAssetFromVideoAtFileURL: on PHAssetChangeRequest from the Photos framework to create a new asset instead

## Parameters 

`videoPathURL`  

An URL that specifies the location of video data.

`completionBlock`  

The block invoked after the save operation completes.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeModifiedVideoAtPath(toSavedPhotosAlbum videoPathURL: URL!) async throws -> URL?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method saves the video at `videoPathURL` to the Saved Photos album as a new asset that is considered a modified version of the receiver.

## See Also

### Saving to the Saved Photos Album

func writeModifiedImageData(toSavedPhotosAlbum: Data!, metadata: [AnyHashable : Any]!, completionBlock: ALAssetsLibraryWriteImageCompletionBlock!)

Saves image data to the Saved Photos album.

Deprecated

