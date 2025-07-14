

- Foundation
- URL
-  init(filePath:directoryHint:relativeTo:) 

Initializer

# init(filePath:directoryHint:relativeTo:)

Creates a file URL that references a path you specify as a string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    filePath path: String,
    directoryHint: URL.DirectoryHint = .inferFromPath,
    relativeTo base: URL? = nil
)
```

## Parameters 

`path`  

The location in the file system, as a string.

`directoryHint`  

A hint to the initializer to indicate whether the path is a directory, or to instruct the initializer to make this determination.

`base`  

A URL that provides a file system location that the path extends.

## Mentioned in 

Improving performance and stability when accessing the file system

## See Also

### Creating a file URL from a string path

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

init(fileURLWithFileSystemRepresentation: UnsafePointer&lt;Int8>, isDirectory: Bool, relativeTo: URL?)

Creates a file URL that references the local file or directory for the file system representation of the path.

init(fileReferenceLiteralResourceName: String)

Creates a URL from a playground file literal.

init?(filePath: FilePath, directoryHint: URL.DirectoryHint)

Creates a file URL that references a file path.

