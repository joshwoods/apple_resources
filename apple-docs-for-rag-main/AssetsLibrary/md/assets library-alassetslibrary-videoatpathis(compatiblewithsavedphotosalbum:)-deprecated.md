

- Assets Library
- ALAssetsLibrary
-  videoAtPathIs(compatibleWithSavedPhotosAlbum:) Deprecated

Instance Method

# videoAtPathIs(compatibleWithSavedPhotosAlbum:)

Returns a Boolean value that indicates whether a video identified by a given URL is compatible with the Saved Photos album.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func videoAtPathIs(compatibleWithSavedPhotosAlbum videoPathURL: URL!) -> Bool
```

Deprecated

Use isCompatibleWithSavedPhotosAlbum on AVAsset instead

## Parameters 

`videoPathURL`  

An URL that points to a video file.

## Return Value

true if the video identified by `videoPathURL` is compatible with the Saved Photos album, otherwise false.

## Discussion

This method returns the same value as UIVideoAtPathIsCompatibleWithSavedPhotosAlbum(_:) would for the same URL.

## See Also

### Saving Assets

func writeVideoAtPath(toSavedPhotosAlbum: URL!, completionBlock: ALAssetsLibraryWriteVideoCompletionBlock!)

Saves a video identified by a given URL to the Saved Photos album.

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

