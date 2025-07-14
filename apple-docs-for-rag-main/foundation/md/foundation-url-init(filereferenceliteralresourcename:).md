

- Foundation
- URL
-  init(fileReferenceLiteralResourceName:) 

Initializer

# init(fileReferenceLiteralResourceName:)

Creates a URL from a playground file literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(fileReferenceLiteralResourceName name: String)
```

## Parameters 

`name`  

The playground file literal name, as a string.

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

init(fileURLWithFileSystemRepresentation: UnsafePointer&lt;Int8>, isDirectory: Bool, relativeTo: URL?)

Creates a file URL that references the local file or directory for the file system representation of the path.

init?(filePath: FilePath, directoryHint: URL.DirectoryHint)

Creates a file URL that references a file path.

