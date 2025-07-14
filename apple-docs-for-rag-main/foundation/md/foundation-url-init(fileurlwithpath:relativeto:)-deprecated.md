

- Foundation
- URL
-  init(fileURLWithPath:relativeTo:) Deprecated

Initializer

# init(fileURLWithPath:relativeTo:)

Creates a file URL that references the local file or directory at the given path, relative to a base URL.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 8.0–18.4DeprecatedmacOS 10.10–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
init(
    fileURLWithPath path: String,
    relativeTo base: URL?
)
```

Deprecated

Use init(filePath:directoryHint:relativeTo:) instead.

## Parameters 

`path`  

The location in the file system.

`base`  

A URL that provides a file system location that the path extends.

## Discussion

If the path is an empty string, the system interprets it as “.”.

This method may perform file system I/O to determine if the path is to a directory. If you know the path is to a directory, use init(fileURLWithPath:isDirectory:relativeTo:) to avoid the file system I/O.

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

init(fileURLWithPath: String, isDirectory: Bool, relativeTo: URL?)

Creates a file URL that references the local file or directory at the given path, relative to a base URL.

Deprecated

init(fileURLWithFileSystemRepresentation: UnsafePointer&lt;Int8>, isDirectory: Bool, relativeTo: URL?)

Creates a file URL that references the local file or directory for the file system representation of the path.

init(fileReferenceLiteralResourceName: String)

Creates a URL from a playground file literal.

init?(filePath: FilePath, directoryHint: URL.DirectoryHint)

Creates a file URL that references a file path.

