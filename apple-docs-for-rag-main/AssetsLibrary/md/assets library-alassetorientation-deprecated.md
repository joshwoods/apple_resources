

- Assets Library
-  ALAssetOrientation Deprecated

Enumeration

# ALAssetOrientation

Constants to indicate the orientation of an asset.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
enum ALAssetOrientation
```

Deprecated

Use UIImageOrientation in the Photos framework instead

## Topics

### Constants

case up

Indicates that the picture is in its default orientation.

case down

Indicates that the picture has been rotated through 180 degrees with respect to the up orientation.

case left

Indicates that the picture has been rotated through 90 degrees counter-clockwise with respect to the up orientation.

case right

Indicates that the picture has been rotated through 90 degrees clockwise with respect to the up orientation.

case upMirrored

Indicates that the picture has been flipped horizontally with respect to the up orientation.

case downMirrored

Indicates that the picture has been rotated through 180 degrees with respect to up orientation, and then flipped horizontally.

case leftMirrored

Indicates that the picture has been rotated through 90 degrees counter-clockwise with respect to the up orientation, and then flipped vertically.

case rightMirrored

Indicates that the picture has been rotated through 90 degrees clockwise with respect to the up orientation and then flipped vertically.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

typealias ALAssetsGroupType

A bitfield to identify types of asset.

Deprecated

Types of Asset

Constants to identify types of asset.

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

