

- File Provider
-  NSFileProviderItemVersion 

Class

# NSFileProviderItemVersion

The version of the item’s content and its metadata.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
class NSFileProviderItemVersion
```

## Overview

Each item has a separate version object for its metadata and its content. As a result, the file provider can update an item’s metadata without uploading or downloading a new copy of its content.

## Topics

### Creating Version Instances

init(contentVersion: Data, metadataVersion: Data)

Creates a new version object.

### Accessing Version Data

class var beforeFirstSyncComponent: Data

A Boolean value indicating that this version predates the version returned by the file provider extension.

var contentVersion: Data

An opaque object used to track versions of the item’s content.

var metadataVersion: Data

An opaque object used to track versions of the item’s metadata.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Items and metadata

struct NSFileProviderItemFields

Fields that specify which of the item’s properties have changed.

class NSFileProviderRequest

An object that provides information about the application requesting data from the File Provider extension.

protocol NSFileProviderItemDecorating

Support for decorating items.

struct NSFileProviderItemDecorationIdentifier

A decoration identifier defined in the File Provider extension’s information property list.

