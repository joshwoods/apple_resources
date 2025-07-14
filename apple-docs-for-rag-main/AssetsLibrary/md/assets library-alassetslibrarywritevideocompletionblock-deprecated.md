

- Assets Library
-  ALAssetsLibraryWriteVideoCompletionBlock Deprecated

Type Alias

# ALAssetsLibraryWriteVideoCompletionBlock

Signature for the block executed when writeVideoAtPath(toSavedPhotosAlbum:completionBlock:) completes.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
typealias ALAssetsLibraryWriteVideoCompletionBlock = (URL?, (any Error)?) -> Void
```

Deprecated

Use performChanges:completionHandler: or performChangesAndWait: on the shared PHPhotoLibrary with a PHAssetChangeRequest from the Photos framework instead

## Discussion

The block parameters are defined as follows:

assetURL  
An URL that identifies the saved video file.

If the video is not saved, `assetURL` is `nil`.

error  
If the video is not saved, an error object that describes the reason for failure, otherwise `nil`.

## See Also

### Constants

typealias ALAssetsGroupType

A bitfield to identify types of asset.

Deprecated

Types of Asset

Constants to identify types of asset.

enum ALAssetOrientation

Constants to indicate the orientation of an asset.

Deprecated

typealias ALAssetsLibraryGroupsEnumerationResultsBlock

Signature for the block executed when a match is found during enumeration using enumerateGroups(withTypes:using:failureBlock:).

Deprecated

typealias ALAssetsLibraryAssetForURLResultBlock

Signature for the block executed if the user has granted access to the caller to access the data managed by the framework in asset(for:resultBlock:failureBlock:).

Deprecated

typealias ALAssetsLibraryWriteImageCompletionBlock

Signature for the block executed when writeImage(toSavedPhotosAlbum:orientation:completionBlock:) completes.

Deprecated

typealias ALAssetsLibraryAccessFailureBlock

Signature for the block executed if the user does not grant access to the caller to access the data managed by the framework.

Deprecated

typealias ALAssetsLibraryGroupResultBlock

Signature for the block executed if the user grants access to the caller to access the data managed by the framework..

Deprecated

enum ALAuthorizationStatus

Constants to indicate authorization status.

Deprecated

Notification Keys

Keys used to get values from the user information dictionary of the ALAssetsLibraryChangedNotification notification.

Error Domain

Constant for the AssetsLibrary domain.

Error Codes

AssetsLibrary-related error codes

