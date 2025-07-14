

- Assets Library
-  ALAssetsLibraryAccessFailureBlock Deprecated

Type Alias

# ALAssetsLibraryAccessFailureBlock

Signature for the block executed if the user does not grant access to the caller to access the data managed by the framework.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
typealias ALAssetsLibraryAccessFailureBlock = ((any Error)?) -> Void
```

Deprecated

Use the Photos framework instead

## Discussion

The block parameter is defined as follows:

error  
An error object that describes why access to the library failed.

This block type is used by asset(for:resultBlock:failureBlock:) and enumerateGroups(withTypes:using:failureBlock:).

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

typealias ALAssetsLibraryWriteVideoCompletionBlock

Signature for the block executed when writeVideoAtPath(toSavedPhotosAlbum:completionBlock:) completes.

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

