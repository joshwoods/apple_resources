

- File Provider
-  NSFileProviderItemProtocol 

Protocol

# NSFileProviderItemProtocol

A protocol that defines the properties of an item managed by the File Provider extension.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderItemProtocol : NSObjectProtocol
```

## Mentioned in 

Synchronizing the File Provider Extension

## Overview

Most of these properties are optional. A File Provider extension doesn’t need to implement all properties for all items.

## Topics

### Providing Required Properties

var itemIdentifier: NSFileProviderItemIdentifier

The item’s persistent identifier.

**Required**

var filename: String

The item’s filename.

**Required**

var typeIdentifier: String

The item’s Uniform Type Identifier (UTI).

Deprecated

var contentType: UTType

The item’s Uniform Type Identifier (UTI).

var capabilities: NSFileProviderItemCapabilities

The item’s capabilities.

### Managing Content

var childItemCount: NSNumber?

The number of items contained by this item.

var documentSize: NSNumber?

The document’s size, in bytes.

var contentPolicy: NSFileProviderContentPolicy

enum NSFileProviderContentPolicy

### Specifying Content Location

var parentItemIdentifier: NSFileProviderItemIdentifier

The persistent identifier of the item’s parent folder.

**Required**

var isTrashed: Bool

A Boolean value that indicates whether an item is in the trash.

var symlinkTargetPath: String?

The target of the symlink.

### Tracking Usage

var contentModificationDate: Date?

The date the item was last modified.

var creationDate: Date?

The date the item was created.

var lastUsedDate: Date?

The date the item was last used.

### Tracking Versions

var itemVersion: NSFileProviderItemVersion

A version object that tracks changes to an item.

var versionIdentifier: Data?

A data value used to determine when the item changes.

var isMostRecentVersionDownloaded: Bool

A Boolean value that indicates whether the item is the most recent version downloaded from the server.

### Monitoring File Transfers

var isUploading: Bool

A Boolean value that indicates whether the item is currently uploading to your remote server.

var isUploaded: Bool

A Boolean value that indicates whether the item has been uploaded to your remote server.

var uploadingError: (any Error)?

An object describing an error that occurred while uploading the item.

var isDownloading: Bool

A Boolean value that indicates whether the item is currently downloading from your remote server.

var isDownloaded: Bool

A Boolean value that indicates whether the item has been downloaded from your remote server.

var downloadingError: (any Error)?

An object describing an error that occurred while downloading the item.

### Sharing

var isShared: Bool

A Boolean value that indicates whether the item is shared with other users.

var isSharedByCurrentUser: Bool

A Boolean value that indicates whether the item was shared by the current user.

var mostRecentEditorNameComponents: PersonNameComponents?

The most recent editor’s name.

var ownerNameComponents: PersonNameComponents?

The name of the item’s owner.

### Managing Metadata

var extendedAttributes: [String : Data]

The extended file attributes synced by the File Provider extension.

var fileSystemFlags: NSFileProviderFileSystemFlags

Flags that define an item’s on-disk properties and its appearance in the user interface.

struct NSFileProviderFileSystemFlags

Flags that define an item’s on-disk properties and its appearance in the user interface.

var tagData: Data?

An abstract data blob representing the tags associated with the item.

var userInfo: [AnyHashable : Any]?

A property list that contains additional data about the item.

var favoriteRank: NSNumber?

A 64-bit, unsigned integer indicating the order of the favorite item in the Favorites list.

let NSFileProviderFavoriteRankUnranked: UInt64

A value that indicates that the item is not ranked.

var typeAndCreator: NSFileProviderTypeAndCreator

The file type and creator codes for the item.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSFileProviderItemDecorating

## See Also

### Provided items

typealias NSFileProviderItem

An item the File Provider extension manages.

struct NSFileProviderItemIdentifier

A unique identifier for an item managed by the File Provider extension.

struct NSFileProviderItemCapabilities

An item’s capabilities, which define the actions that the user can perform in the document browser.

struct NSFileProviderTypeAndCreator

A structure that contains the file type and file creator codes for an item.

