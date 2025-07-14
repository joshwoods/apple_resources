

- Foundation
- URL
-  isFileURL 

Instance Property

# isFileURL

A Boolean that is true if the scheme is `file:`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isFileURL: Bool { get }
```

## See Also

### Working with file URLs

var hasDirectoryPath: Bool

A Boolean that is true if the URL path represents a directory.

func withUnsafeFileSystemRepresentation&lt;ResultType>((UnsafePointer&lt;Int8>?) throws -> ResultType) rethrows -> ResultType

Passes the URL’s path in the file system representation to a closure.

func resolveSymlinksInPath()

Resolves any symlinks in the path of a file URL.

func resolvingSymlinksInPath() -> URL

Resolves any symlinks in the path of a file URL.

func standardize()

Standardizes the path of a file URL.

