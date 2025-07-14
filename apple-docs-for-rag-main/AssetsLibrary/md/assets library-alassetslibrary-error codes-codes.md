

- Assets Library
- ALAssetsLibrary
-  Error Codes 

API Collection

# Error Codes

AssetsLibrary-related error codes

## Topics

### Constants

var ALAssetsLibraryUnknownError: Int

The reason for the error is unknown.

var ALAssetsLibraryWriteFailedError: Int

The attempt to write data failed.

var ALAssetsLibraryWriteBusyError: Int

Writing was already busy when the attempt to write was made.

var ALAssetsLibraryWriteInvalidDataError: Int

The data was invalid.

var ALAssetsLibraryWriteIncompatibleDataError: Int

The data contained incompatible data.

var ALAssetsLibraryWriteDataEncodingError: Int

The data contained data with the wrong encoding.

var ALAssetsLibraryWriteDiskSpaceError: Int

There was not enough space on the disk to write the data.

var ALAssetsLibraryDataUnavailableError: Int

The data was not available.

var ALAssetsLibraryAccessUserDeniedError: Int

The user denied access to the library.

var ALAssetsLibraryAccessGloballyDeniedError: Int

Access to the library was denied globally.

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

