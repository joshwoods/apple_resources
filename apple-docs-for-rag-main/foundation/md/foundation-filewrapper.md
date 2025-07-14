

- Foundation
-  FileWrapper 

Class

# FileWrapper

A representation of a node (a file, directory, or symbolic link) in the file system.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class FileWrapper
```

## Overview

The FileWrapper class provides access to the attributes and contents of file system nodes. A file system node is a file, directory, or symbolic link. Instances of this class are known as file wrappers.

Note

Starting in macOS 10.7, FileWrapper moved from Application Kit to Foundation. As a result of this the `icon`, and `setIcon:` methods have moved to a new category of FileWrapper that remains in Application Kit.

File wrappers represent a file system node as an object that can be displayed as an image (and possibly edited in place), saved to the file system, or transmitted to another application.

There are three types of file wrappers:

- Regular-file file wrapper: Represents a regular file.

- Directory file wrapper: Represents a directory.

- Symbolic-link file wrapper: Represents a symbolic link.

A file wrapper has these attributes:

- Filename. Name of the file system node the file wrapper represents.

- file-system attributes. See FileManager for information on the contents of the `attributes` dictionary.

- Regular-file contents. Applicable only to regular-file file wrappers.

- File wrappers. Applicable only to directory file wrappers.

- Destination node. Applicable only to symbolic-link file wrappers.

## Topics

### Creating File Wrappers

This class has several designated initializers.

init(url: URL, options: FileWrapper.ReadingOptions) throws

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the URL.

convenience init?(path: String)

Initializes a file wrapper instance whose kind is determined by the type of file-system node located by the path.

Deprecated

init(directoryWithFileWrappers: [String : FileWrapper])

Initializes the receiver as a directory file wrapper, with a given file-wrapper list.

init(regularFileWithContents: Data)

Initializes the receiver as a regular-file file wrapper.

convenience init(symbolicLinkWithDestination: String)

Initializes the receiver as a symbolic-link file wrapper.

Deprecated

init(symbolicLinkWithDestinationURL: URL)

Initializes the receiver as a symbolic-link file wrapper that links to a specified file.

init?(serializedRepresentation: Data)

Initializes the receiver as a regular-file file wrapper from given serialized data.

### Querying File Wrappers

var isRegularFile: Bool

This property contains a boolean value that indicates whether the file wrapper object is a regular-file.

var isDirectory: Bool

This property contains a boolean value indicating whether the file wrapper is a directory file wrapper.

var isSymbolicLink: Bool

A boolean that indicates whether the file wrapper object is a symbolic-link file wrapper.

### Accessing File-Wrapper Information

var fileWrappers: [String : FileWrapper]?

The file wrappers contained by a directory file wrapper.

func addFileWrapper(FileWrapper) -> String

Adds a child file wrapper to the receiver, which must be a directory file wrapper.

func removeFileWrapper(FileWrapper)

Removes a child file wrapper from the receiver, which must be a directory file wrapper.

func addFile(withPath: String) -> String

Creates a file wrapper from a given file-system node and adds it to the receiver, which must be a directory file wrapper.

Deprecated

func addRegularFile(withContents: Data, preferredFilename: String) -> String

Creates a regular-file file wrapper with the given contents and adds it to the receiver, which must be a directory file wrapper.

func addSymbolicLink(withDestination: String, preferredFilename: String) -> String

Creates a symbolic-link file wrapper pointing to a given file-system node and adds it to the receiver, which must be a directory file wrapper.

Deprecated

func keyForChildFileWrapper(FileWrapper) -> String?

Returns the dictionary key used by a directory to identify a given file wrapper.

func symbolicLinkDestination() -> String

Provides the pathname referenced by the file wrapper object, which must be a symbolic-link file wrapper.

Deprecated

var symbolicLinkDestinationURL: URL?

The URL referenced by the file wrapper object, which must be a symbolic-link file wrapper.

### Updating File Wrappers

func needsToBeUpdated(fromPath: String) -> Bool

Indicates whether the file wrapper needs to be updated to match a given file-system node.

Deprecated

func matchesContents(of: URL) -> Bool

Indicates whether the contents of a file wrapper matches a directory, regular file, or symbolic link on disk.

func update(fromPath: String) -> Bool

Updates the file wrapper to match a given file-system node.

Deprecated

func read(from: URL, options: FileWrapper.ReadingOptions) throws

Recursively rereads the entire contents of a file wrapper from the specified location on disk.

### Serializing

var serializedRepresentation: Data?

The contents of the file wrapper as an opaque data object.

### Accessing Files

var filename: String?

The filename of the file wrapper object

var preferredFilename: String?

The preferred filename for the file wrapper object.

var fileAttributes: [String : Any]

A dictionary of file attributes.

var regularFileContents: Data?

The contents of the file-system node associated with a regular-file file wrapper.

### Writing Files

func write(toFile: String, atomically: Bool, updateFilenames: Bool) -> Bool

Writes a file wrapper’s contents to a given file-system node.

Deprecated

func write(to: URL, options: FileWrapper.WritingOptions, originalContentsURL: URL?) throws

Recursively writes the entire contents of a file wrapper to a given file-system URL.

### Working with Icons

var icon: NSImage?

The icon that represents the file wrapper.

### Constants

struct ReadingOptions

Reading options that can be set by the init(url:options:) and read(from:options:) methods.

struct WritingOptions

Writing options that can be set by the write(to:options:originalContentsURL:) method.

### Initializers

init?(coder: NSCoder)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Managed file access

class FileHandle

An object-oriented wrapper for a file descriptor.

class NSFileSecurity

A stub class that encapsulates security information about a file.

class NSFileVersion

A snapshot of a file at a specific point in time.

