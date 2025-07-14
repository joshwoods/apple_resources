

- File Provider
-  NSFileProviderItemFields 

Structure

# NSFileProviderItemFields

Fields that specify which of the item’s properties have changed.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
struct NSFileProviderItemFields
```

## Overview

Most of the fields correspond to properties in the NSFileProviderItemProtocol protocol.

## Topics

### Specifying the Required Fields

static var filename: NSFileProviderItemFields

The item’s filename.

static var contents: NSFileProviderItemFields

The item’s content.

### Specifying Content Location

static var parentItemIdentifier: NSFileProviderItemFields

The identity of the directory that contains the item.

### Tracking Usage

static var contentModificationDate: NSFileProviderItemFields

The item’s modification date.

static var creationDate: NSFileProviderItemFields

The item’s creation date.

static var lastUsedDate: NSFileProviderItemFields

The date the item was last used.

### Working with Metadata

static var extendedAttributes: NSFileProviderItemFields

The item’s extended attributes.

static var fileSystemFlags: NSFileProviderItemFields

The flags describing the item’s on-disk representation.

static var tagData: NSFileProviderItemFields

The tags for the item.

static var favoriteRank: NSFileProviderItemFields

The item’s favorite rank.

static var typeAndCreator: NSFileProviderItemFields

The file type and creator codes for the item.

### Initializers

init(rawValue: UInt)

Creates an option instance from the raw value.

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

### Items and metadata

class NSFileProviderItemVersion

The version of the item’s content and its metadata.

class NSFileProviderRequest

An object that provides information about the application requesting data from the File Provider extension.

protocol NSFileProviderItemDecorating

Support for decorating items.

struct NSFileProviderItemDecorationIdentifier

A decoration identifier defined in the File Provider extension’s information property list.

