

- Foundation
- URL
-  withUnsafeFileSystemRepresentation(\_:) 

Instance Method

# withUnsafeFileSystemRepresentation(\_:)

Passes the URL’s path in the file system representation to a closure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withUnsafeFileSystemRepresentation(_ block: (UnsafePointer?) throws -> ResultType) rethrows -> ResultType
```

## Parameters 

`block`  

A closure to execute, which receives a C string as its parameter, and returns a value of a type you choose.

The parameter passed to the closure is `nil` if the URL cannot be represented by the file system. For example, if the URL contains an accented character and the file system only supports ASCII, no file system representation is possible.

## Return Value

The value returned by your closure, if any.

## Discussion

The file system representation is a null-terminated C string with canonical UTF-8 encoding.

Note

The pointer is not valid outside the context of the closure.

## See Also

### Working with file URLs

var isFileURL: Bool

A Boolean that is true if the scheme is `file:`.

var hasDirectoryPath: Bool

A Boolean that is true if the URL path represents a directory.

func resolveSymlinksInPath()

Resolves any symlinks in the path of a file URL.

func resolvingSymlinksInPath() -> URL

Resolves any symlinks in the path of a file URL.

func standardize()

Standardizes the path of a file URL.

