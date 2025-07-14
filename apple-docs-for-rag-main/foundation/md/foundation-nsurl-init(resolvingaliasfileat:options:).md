

- Foundation
- NSURL
-  init(resolvingAliasFileAt:options:) 

Initializer

# init(resolvingAliasFileAt:options:)

Returns a new URL made by resolving the alias file at `url`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    resolvingAliasFileAt url: URL,
    options: NSURL.BookmarkResolutionOptions = []
) throws
```

## Parameters 

`url`  

The URL pointing to the alias file.

`options`  

Options taken into account when resolving the bookmark data. The withSecurityScope option is not supported by this method.

## Return Value

A new URL created by resolving the bookmark data derived from the provided alias file. If an error occurs, this method returns `nil`.

## Discussion

Creates and initializes a new URL based on the alias file at `url`. Use this method to resolve bookmark data that was saved using writeBookmarkData(_:to:options:) and resolves that data in one step.

If the `url` argument does not refer to an alias file as defined by the `NSURLIsAliasFileKey` property, this method returns the `url` argument.

If the `url` argument is unreachable, this method returns `nil` and the optional error argument is populated.

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

convenience init(resolvingBookmarkData: Data, options: NSURL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: UnsafeMutablePointer&lt;ObjCBool>?) throws

Initializes a newly created NSURL that points to a location specified by resolving bookmark data.

class func fileURL(withFileSystemRepresentation: UnsafePointer&lt;CChar>, isDirectory: Bool, relativeTo: URL?) -> URL

Returns a new URL object initialized with a C string representing a local file system path.

func getFileSystemRepresentation(UnsafeMutablePointer&lt;CChar>, maxLength: Int) -> Bool

Fills the provided buffer with a C string representing a local file system path.

