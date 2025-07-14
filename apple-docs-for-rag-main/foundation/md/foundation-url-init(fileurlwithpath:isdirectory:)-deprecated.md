

- Foundation
- URL
-  init(fileURLWithPath:isDirectory:) Deprecated

Initializer

# init(fileURLWithPath:isDirectory:)

Creates a file URL that references the local file or directory at the given path.

iOS 8.0–18.4DeprecatediPadOS 8.0–18.4DeprecatedMac Catalyst 8.0–18.4DeprecatedmacOS 10.10–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
init(
    fileURLWithPath path: String,
    isDirectory: Bool
)
```

Deprecated

Use init(filePath:directoryHint:relativeTo:) instead.

## Parameters 

`path`  

The location in the file system.

`isDirectory`  

A Boolean value that indicates whether the location is a directory.

## Discussion

If the path is an empty string, the system interprets it as “.”.

Note

This method avoids file system I/O to determine if the path is to a directory. When you know that information, prefer this method to initializers without the parameter.

## See Also

### Creating a file URL from a string path

init(filePath: String, directoryHint: URL.DirectoryHint, relativeTo: URL?)

Creates a file URL that references a path you specify as a string.

enum DirectoryHint

A hint to URL file APIs for handling paths that may reference directories.

init(fileURLWithPath: String)

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

