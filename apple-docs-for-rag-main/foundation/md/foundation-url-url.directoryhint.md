

- Foundation
- URL
-  URL.DirectoryHint 

Enumeration

# URL.DirectoryHint

A hint to URL file APIs for handling paths that may reference directories.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum DirectoryHint
```

## Topics

### Hints

case isDirectory

A hint that specifies that a given path is a directory.

case notDirectory

A hint that specifies that a given path isn’t a directory.

case checkFileSystem

A hint that directs a URL call to consult the file system to determine whether the path references a directory.

case inferFromPath

A hint that directs a URL call to infer whether a path references a directory based on whether it has a trailing slash.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a file URL from a string path

init(filePath: String, directoryHint: URL.DirectoryHint, relativeTo: URL?)

Creates a file URL that references a path you specify as a string.

init(fileURLWithPath: String)

Creates a file URL that references the local file or directory at the given path.

Deprecated

init(fileURLWithPath: String, isDirectory: Bool)

Creates a file URL that references the local file or directory at the given path.

Deprecated

init(fileURLWithPath: String, relativeTo: URL?)

Creates a file URL that references the local file or directory at the given path, relative to a base URL.

Deprecated

init(fileURLWithPath: String, isDirectory: Bool, relativeTo: URL?)

Creates a file URL that references the local file or directory at the given path, relative to a base URL.

Deprecated

init(fileURLWithFileSystemRepresentation: UnsafePointer&lt;Int8>, isDirectory: Bool, relativeTo: URL?)

Creates a file URL that references the local file or directory for the file system representation of the path.

init(fileReferenceLiteralResourceName: String)

Creates a URL from a playground file literal.

init?(filePath: FilePath, directoryHint: URL.DirectoryHint)

Creates a file URL that references a file path.

