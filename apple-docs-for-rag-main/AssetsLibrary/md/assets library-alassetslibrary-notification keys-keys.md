

- Assets Library
- ALAssetsLibrary
-  Notification Keys 

API Collection

# Notification Keys

Keys used to get values from the user information dictionary of the ALAssetsLibraryChangedNotification notification.

## Overview

Assets that are modified use the ALAssetLibraryUpdatedAssetsKey key. Assets that are inserted or deleted use the ALAssetLibraryUpdatedAssetGroupsKey key for the asset group that contains the asset.

Assets and asset groups that have no strong references are omitted from the notification’s user information dictionary.

## Topics

### Constants

let ALAssetLibraryUpdatedAssetsKey: String

Value is a set of NSURL objects identifying the assets that were updated.

Deprecated

let ALAssetLibraryInsertedAssetGroupsKey: String

Value is a set of NSURL objects identifying the assets that were inserted.

Deprecated

let ALAssetLibraryUpdatedAssetGroupsKey: String

Value is a set of NSURL objects identifying the asset groups that were updated.

Deprecated

let ALAssetLibraryDeletedAssetGroupsKey: String

Value is a set of NSURL objects identifying the asset groups that were deleted.

Deprecated

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

Error Domain

Constant for the AssetsLibrary domain.

Error Codes

AssetsLibrary-related error codes

