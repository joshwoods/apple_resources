

- Foundation
- NSURL
-  init(string:relativeTo:) 

Initializer

# init(string:relativeTo:)

Initializes an NSURL object with a base URL and a relative string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    string URLString: String,
    relativeTo baseURL: URL?
)
```

## Parameters 

`URLString`  

The URL string with which to initialize the NSURL object. Linked on or after iOS 17, this method parses `URLString` according to RFC 3986. Linked before iOS 17, this method parses `URLString` according to RFCs 1738 and 1808. `URLString` is interpreted relative to `baseURL`.

`baseURL`  

The base URL for the NSURL object.

## Return Value

An NSURL object initialized with `URLString` and `baseURL`. If `URLString` was malformed, returns `nil`.

## Discussion

This method allows you to create a URL relative to a base path or URL. For example, if you have the URL for a folder on disk and the name of a file within that folder, you can construct a URL for the file by providing the folder’s URL as the base path (with a trailing slash) and the filename as the string part.

Important

For apps linked on or after iOS 17 and aligned OS versions, NSURL parsing has updated from the obsolete RFC 1738/1808 parsing to the same RFC 3986 parsing as NSURLComponents. This unifies the parsing behaviors of the `NSURL` and `NSURLComponents` APIs. Now, `NSURL` automatically percent- and IDNA-encodes invalid characters to help create a valid URL.

To check if `URLString` is strictly valid according to the RFC, use the new `[NSURL URLWithString:URLString encodingInvalidCharacters:NO]` method. This method leaves all characters as they are and returns `nil` if `URLString` is explicitly invalid.

For apps linked before iOS 17, this method expects `URLString` to contain only characters that are allowed in a properly formed URL. All other characters must be properly percent encoded. Any percent-encoded characters are interpreted using UTF-8 encoding.

init(string:relativeTo:) is the designated initializer for NSURL.

## See Also

### Related Documentation

class NSURL

An object that represents the location of a resource, such as an item on a remote server or the path to a local file.

### Creating a URL object

convenience init?(string: String)

Initializes an NSURL object with a provided URL string.

convenience init?(string: String, encodingInvalidCharacters: Bool)

Creates an instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

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

convenience init(resolvingBookmarkData: Data, options: NSURL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: UnsafeMutablePointer&lt;ObjCBool>?) throws

Initializes a newly created NSURL that points to a location specified by resolving bookmark data.

class func fileURL(withFileSystemRepresentation: UnsafePointer&lt;CChar>, isDirectory: Bool, relativeTo: URL?) -> URL

Returns a new URL object initialized with a C string representing a local file system path.

func getFileSystemRepresentation(UnsafeMutablePointer&lt;CChar>, maxLength: Int) -> Bool

Fills the provided buffer with a C string representing a local file system path.

