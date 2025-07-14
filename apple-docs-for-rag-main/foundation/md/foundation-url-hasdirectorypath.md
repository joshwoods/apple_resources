

- Foundation
- URL
-  hasDirectoryPath 

Instance Property

# hasDirectoryPath

A Boolean that is true if the URL path represents a directory.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hasDirectoryPath: Bool { get }
```

## See Also

### Working with file URLs

var isFileURL: Bool

A Boolean that is true if the scheme is `file:`.

func withUnsafeFileSystemRepresentation&lt;ResultType>((UnsafePointer&lt;Int8>?) throws -> ResultType) rethrows -> ResultType

Passes the URL’s path in the file system representation to a closure.

func resolveSymlinksInPath()

Resolves any symlinks in the path of a file URL.

func resolvingSymlinksInPath() -> URL

Resolves any symlinks in the path of a file URL.

func standardize()

Standardizes the path of a file URL.

