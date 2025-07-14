

- Foundation
-  FileProtectionType 

Structure

# FileProtectionType

Protection level values that can be associated with a file attribute key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct FileProtectionType
```

## Overview

These values are associated with the protectionKey key.

## Topics

### Creating a File Protection Type

init(rawValue: String)

### Working with Protection Levels

static let complete: FileProtectionType

The file is stored in an encrypted format on disk and cannot be read from or written to while the device is locked or booting.

static let completeUnlessOpen: FileProtectionType

The file is stored in an encrypted format on disk after it is closed.

static let completeUntilFirstUserAuthentication: FileProtectionType

The file is stored in an encrypted format on disk and cannot be accessed until after the device has booted.

static let none: FileProtectionType

The file has no special protections associated with it.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

struct DirectoryEnumerationOptions

Options for enumerating the contents of directories.

enum SearchPathDirectory

The location of significant directories.

struct SearchPathDomainMask

Domain constants specifying base locations to use when you search for significant directories.

struct FileAttributeKey

Keys in dictionaries used to get and set file attributes.

struct FileAttributeType

Values representing a file’s type attribute.

struct URLFileProtection

Protection-level values for a URL resource key.

