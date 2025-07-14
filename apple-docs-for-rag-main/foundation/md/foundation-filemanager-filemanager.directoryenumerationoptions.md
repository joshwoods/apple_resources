

- Foundation
- FileManager
-  FileManager.DirectoryEnumerationOptions 

Structure

# FileManager.DirectoryEnumerationOptions

Options for enumerating the contents of directories.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct DirectoryEnumerationOptions
```

## Overview

These options are used with the contentsOfDirectory(at:includingPropertiesForKeys:options:) method.

## Topics

### Creating a Directory Enumeration Options Value

init(rawValue: UInt)

### Directory Enumeration Options

static var skipsSubdirectoryDescendants: FileManager.DirectoryEnumerationOptions

An option to perform a shallow enumeration that doesn’t descend into directories.

static var skipsPackageDescendants: FileManager.DirectoryEnumerationOptions

An option to treat packages like files and not descend into their contents.

static var skipsHiddenFiles: FileManager.DirectoryEnumerationOptions

An option to skip hidden files.

### Type Properties

static var includesDirectoriesPostOrder: FileManager.DirectoryEnumerationOptions

static var producesRelativePathURLs: FileManager.DirectoryEnumerationOptions

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

enum SearchPathDirectory

The location of significant directories.

struct SearchPathDomainMask

Domain constants specifying base locations to use when you search for significant directories.

struct FileAttributeKey

Keys in dictionaries used to get and set file attributes.

struct FileAttributeType

Values representing a file’s type attribute.

struct FileProtectionType

Protection level values that can be associated with a file attribute key.

struct URLFileProtection

Protection-level values for a URL resource key.

