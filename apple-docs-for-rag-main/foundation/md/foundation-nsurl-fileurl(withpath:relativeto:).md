

- Foundation
- NSURL
-  fileURL(withPath:relativeTo:) 

Type Method

# fileURL(withPath:relativeTo:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func fileURL(
    withPath path: String,
    relativeTo baseURL: URL?
) -> URL
```

## Mentioned in 

Improving performance and stability when accessing the file system

## See Also

### Creating a URL object

convenience init?(string: String)

Initializes an NSURL object with a provided URL string.

convenience init?(string: String, encodingInvalidCharacters: Bool)

Creates an instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init?(string: String, relativeTo: URL?)

Initializes an NSURL object with a base URL and a relative string.

class func fileURL(withPath: String, isDirectory: Bool) -> URL

Initializes and returns a newly created NSURL object as a file URL with a specified path.

init(fileURLWithPath: String, isDirectory: Bool)

Initializes a newly created NSURL referencing the local file or directory at `path`.

init(fileURLWithPath: String, relativeTo: URL?)

class func fileURL(withPath: String, isDirectory: Bool, relativeTo: URL?) -> URL

init(fileURLWithPath: String, isDirectory: Bool, relativeTo: URL?)

class func fileURL(withPath: String) -> URL

Initializes and returns a newly created NSURL object as a file URL with a specified path.

init(fileURLWithPath: String)

Initializes a newly created NSURL referencing the local file or directory at `path`.

class func fileURL(withPathComponents: [String]) -> URL?

Initializes and returns a newly created NSURL object as a file URL with specified path components.

convenience init(resolvingAliasFileAt: URL, options: NSURL.BookmarkResolutionOptions) throws

Returns a new URL made by resolving the alias file at `url`.

convenience init(resolvingBookmarkData: Data, options: NSURL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: UnsafeMutablePointer&lt;ObjCBool>?) throws

Initializes a newly created NSURL that points to a location specified by resolving bookmark data.

class func fileURL(withFileSystemRepresentation: UnsafePointer&lt;CChar>, isDirectory: Bool, relativeTo: URL?) -> URL

Returns a new URL object initialized with a C string representing a local file system path.

func getFileSystemRepresentation(UnsafeMutablePointer&lt;CChar>, maxLength: Int) -> Bool

Fills the provided buffer with a C string representing a local file system path.

