

- Foundation
- URL
-  init(string:relativeTo:) 

Initializer

# init(string:relativeTo:)

Creates a URL instance from the provided string, relative to another URL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    string: String,
    relativeTo url: URL?
)
```

## Parameters 

`string`  

A relative URL location.

`url`  

A URL that provides a base location that the string extends.

## Discussion

Important

For apps linked on or after iOS 17 and aligned OS versions, URL parsing has updated from the obsolete RFC 1738/1808 parsing to the same RFC 3986 parsing as URLComponents. This unifies the parsing behaviors of the `URL` and `URLComponents` APIs. Now, `URL` automatically percent- and IDNA-encodes invalid characters to help create a valid URL.

This initializer returns `nil` if the string doesn’t represent a valid URL even after encoding invalid characters. To check if a URL string is strictly valid according to the RFC, use the new init(string:encodingInvalidCharacters:) initializer and pass `encodingInvalidCharacters: false`. This leaves all characters as they are and returns `nil` if the URL string is explicitly invalid.

## See Also

### Creating a URL from a string

init?(string: String)

Creates a URL instance from the provided string.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Creates a URL that refers to a location specified by resolving bookmark data.

init?(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Initializes a URL that refers to a location specified by resolving bookmark data.

