

- Assets Library
- ALAsset
-  setImageData(\_:metadata:completionBlock:) Deprecated

Instance Method

# setImageData(\_:metadata:completionBlock:)

Replaces the image data in the receiver with given image data

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**iOS, iPadOS, Mac Catalyst**

``` source
func setImageData(
    _ imageData: Data!,
    metadata: [AnyHashable : Any]!,
    completionBlock: ALAssetsLibraryWriteImageCompletionBlock!
)
```

**Mac Catalyst**

``` source
func setImageData(
    _ imageData: Data!,
    metadata: [AnyHashable : Any]!
) async throws -> URL?
```

Deprecated

Use contentEditingOutput on a PHAssetChangeRequest from the Photos framework instead

## Parameters 

`imageData`  

Image data for the asset.

`metadata`  

Metadata for the image.

`completionBlock`  

The block invoked after the save operation completes.

If the application is able to edit the asset, the completion block returns the same asset URL as the receiver, because a new asset is not created.

If the application is not able to edit the asset, the completion blocks return a `nil` asset URL and an `ALAssetsLibraryWriteFailedError`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Before invoking this method, you should check the isEditable property of the asset to determine whether it is possible to replace the image data.

## See Also

### Setting New Image and Video Data

func setVideoAtPath(URL!, completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!)

Replaces the video data in receiver with the video at a given URL.

Deprecated

