

- File Provider
-  NSFileProviderFileSystemFlags 

Structure

# NSFileProviderFileSystemFlags

Flags that define an item’s on-disk properties and its appearance in the user interface.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
struct NSFileProviderFileSystemFlags
```

## Overview

The flags define the on-disk properties of the item. The system modifies the item’s appearance based on these flags.

## Topics

### Flags

static var userReadable: NSFileProviderFileSystemFlags

The user can read the item.

static var userWritable: NSFileProviderFileSystemFlags

The user can modify the item.

static var userExecutable: NSFileProviderFileSystemFlags

The user can execute the item.

static var hidden: NSFileProviderFileSystemFlags

By default, the system hides the item when the user views the file system.

static var pathExtensionHidden: NSFileProviderFileSystemFlags

By default, the system hides the item’s extension when showing its filename.

### Initializers

init(rawValue: UInt)

Creates a new file system flag from the provided value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing Metadata

var extendedAttributes: [String : Data]

The extended file attributes synced by the File Provider extension.

var fileSystemFlags: NSFileProviderFileSystemFlags

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

