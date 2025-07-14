

- Assets Library
- ALAssetsLibrary
-  Types of Asset 

API Collection

# Types of Asset

Constants to identify types of asset.

## Topics

### Constants

var ALAssetsGroupLibrary: UInt32

The Library group that includes all assets that are synced from iTunes.

Deprecated

var ALAssetsGroupAlbum: UInt32

All the albums created on the device or synced from iTunes, not including Photo Stream or Shared Streams

Deprecated

var ALAssetsGroupEvent: UInt32

All events, including those created during Camera Connection Kit import.

Deprecated

var ALAssetsGroupFaces: UInt32

All the faces albums synced from iTunes.

Deprecated

var ALAssetsGroupSavedPhotos: UInt32

All the photos in the Camera Roll.

Deprecated

var ALAssetsGroupPhotoStream: UInt32

The PhotoStream album.

Deprecated

var ALAssetsGroupAll: UInt32

The same as ORing together all the group types except for ALAssetsGroupLibrary.

Deprecated

## See Also

### Constants

typealias ALAssetsGroupType

A bitfield to identify types of asset.

Deprecated

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

Error Codes

AssetsLibrary-related error codes

