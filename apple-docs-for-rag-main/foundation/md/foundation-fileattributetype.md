

- Foundation
-  FileAttributeType 

Structure

# FileAttributeType

Values representing a file’s type attribute.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct FileAttributeType
```

## Discussion

These strings are the possible values for the type attribute key contained in the dictionary object returned by attributesOfItem(atPath:).

## Topics

### Creating a File Attribute Type

init(rawValue: String)

### Accessing File Type Attributes

static let typeBlockSpecial: FileAttributeType

A block special file.

static let typeCharacterSpecial: FileAttributeType

A character special file.

static let typeDirectory: FileAttributeType

A directory.

static let typeRegular: FileAttributeType

A regular file.

static let typeSocket: FileAttributeType

A socket.

static let typeSymbolicLink: FileAttributeType

A symbolic link.

static let typeUnknown: FileAttributeType

A file whose type is unknown.

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

struct FileProtectionType

Protection level values that can be associated with a file attribute key.

struct URLFileProtection

Protection-level values for a URL resource key.

