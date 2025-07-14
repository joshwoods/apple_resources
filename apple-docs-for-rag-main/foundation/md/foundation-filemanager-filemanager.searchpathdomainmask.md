

- Foundation
- FileManager
-  FileManager.SearchPathDomainMask 

Structure

# FileManager.SearchPathDomainMask

Domain constants specifying base locations to use when you search for significant directories.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct SearchPathDomainMask
```

## Overview

These constants are used by the urls(for:in:) and url(for:in:appropriateFor:create:) methods of FileManager.

## Topics

### Creating a Search Path Domain Mask

init(rawValue: UInt)

### Specifying Search Path Domains

static var userDomainMask: FileManager.SearchPathDomainMask

The user’s home directory—the place to install user’s personal items (`~`).

static var localDomainMask: FileManager.SearchPathDomainMask

The place to install items available to everyone on this machine.

static var networkDomainMask: FileManager.SearchPathDomainMask

The place to install items available on the network (`/Network`).

static var systemDomainMask: FileManager.SearchPathDomainMask

A directory for system files provided by Apple (`/System`) .

static var allDomainsMask: FileManager.SearchPathDomainMask

All domains.

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

### Supporting Types

struct DirectoryEnumerationOptions

Options for enumerating the contents of directories.

enum SearchPathDirectory

The location of significant directories.

struct FileAttributeKey

Keys in dictionaries used to get and set file attributes.

struct FileAttributeType

Values representing a file’s type attribute.

struct FileProtectionType

Protection level values that can be associated with a file attribute key.

struct URLFileProtection

Protection-level values for a URL resource key.

