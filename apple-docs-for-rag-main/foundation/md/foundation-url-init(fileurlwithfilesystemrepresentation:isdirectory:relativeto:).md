

- Foundation
- URL
-  init(fileURLWithFileSystemRepresentation:isDirectory:relativeTo:) 

Initializer

# init(fileURLWithFileSystemRepresentation:isDirectory:relativeTo:)

Creates a file URL that references the local file or directory for the file system representation of the path.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    fileURLWithFileSystemRepresentation path: UnsafePointer,
    isDirectory: Bool,
    relativeTo baseURL: URL?
)
```

## Parameters 

`path`  

The location in the file system.

`isDirectory`  

A Boolean value that indicates whether the location is a directory.

`baseURL`  

A URL that provides a file system location that the path extends.

## Discussion

File system representation is a null-terminated C string with canonical UTF-8 encoding.

## See Also

### Creating a file URL from a string path

init(filePath: String, directoryHint: URL.DirectoryHint, relativeTo: URL?)

Creates a file URL that references a path you specify as a string.

enum DirectoryHint

A hint to URL file APIs for handling paths that may reference directories.

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

init(fileReferenceLiteralResourceName: String)

Creates a URL from a playground file literal.

init?(filePath: FilePath, directoryHint: URL.DirectoryHint)

Creates a file URL that references a file path.

