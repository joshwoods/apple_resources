

- FSKit
- FSItem
-  FSItem.Attribute 

Structure

# FSItem.Attribute

A value that indicates a set of item attributes to get or set.

macOS 15.4+

``` source
struct Attribute
```

## Overview

This type is an option set in Swift. In Objective-C, you use the cases of this enumeration to create a bit field.

## Topics

### Working with identifier attributes

static var fileID: FSItem.Attribute

The file ID attribute.

static var parentID: FSItem.Attribute

The parent ID attribute.

### Working with metadata attributes

static var type: FSItem.Attribute

The type attribute.

static var mode: FSItem.Attribute

The mode attribute.

static var linkCount: FSItem.Attribute

The link count attribute.

static var uid: FSItem.Attribute

The user ID (uid) attribute.

static var gid: FSItem.Attribute

The group ID (gid) attribute.

static var flags: FSItem.Attribute

The flags attribute.

static var size: FSItem.Attribute

The size attribute.

static var allocSize: FSItem.Attribute

The allocated size attribute.

static var supportsLimitedXAttrs: FSItem.Attribute

The supports limited extended attributes attribute.

static var inhibitKernelOffloadedIO: FSItem.Attribute

The inhibit kernel offloaded I/O attribute.

### Working with time attributes

static var accessTime: FSItem.Attribute

The last-accessed time attribute.

static var modifyTime: FSItem.Attribute

The last-modified time attribute.

static var changeTime: FSItem.Attribute

The last-changed time attribute.

static var birthTime: FSItem.Attribute

The creation time attribute.

static var backupTime: FSItem.Attribute

The backup time attribute.

static var addedTime: FSItem.Attribute

The time added attribute.

### Working with raw values

init(rawValue: Int)

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

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

### Inspecting requested attributes

var wantedAttributes: FSItem.Attribute

The attributes requested by the request.

func isAttributeWanted(FSItem.Attribute) -> Bool

A method that indicates whether the request wants given attribute.

