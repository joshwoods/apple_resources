

- Foundation
- NSURL
-  init(resolvingBookmarkData:options:relativeTo:bookmarkDataIsStale:) 

Initializer

# init(resolvingBookmarkData:options:relativeTo:bookmarkDataIsStale:)

Initializes a newly created NSURL that points to a location specified by resolving bookmark data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    resolvingBookmarkData bookmarkData: Data,
    options: NSURL.BookmarkResolutionOptions = [],
    relativeTo relativeURL: URL?,
    bookmarkDataIsStale isStale: UnsafeMutablePointer?
) throws
```

## Parameters 

`bookmarkData`  

The bookmark data the URL is derived from.

`options`  

Options taken into account when resolving the bookmark data.

`relativeURL`  

The base URL that the bookmark data is relative to.

`isStale`  

If true, the bookmark data is stale.

## Return Value

An NSURL initialized by resolving `bookmarkData`.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

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

class func fileURL(withPath: String, relativeTo: URL?) -> URL

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

class func fileURL(withFileSystemRepresentation: UnsafePointer&lt;CChar>, isDirectory: Bool, relativeTo: URL?) -> URL

Returns a new URL object initialized with a C string representing a local file system path.

func getFileSystemRepresentation(UnsafeMutablePointer&lt;CChar>, maxLength: Int) -> Bool

Fills the provided buffer with a C string representing a local file system path.

