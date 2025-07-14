

- Foundation
- URL
-  init(string:encodingInvalidCharacters:) 

Initializer

# init(string:encodingInvalidCharacters:)

Creates a URL instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init?(
    string: String,
    encodingInvalidCharacters: Bool
)
```

## Parameters 

`string`  

A URL location.

`encodingInvalidCharacters`  

A Boolean value that indicates whether the initializer attempts to encode any invalid characters in `string`.

## Discussion

If `encodingInvalidCharacters` is `true`, this initializer tries to encode the string to create a valid URL. If the URL string is still invalid after encoding, the initializer returns `nil`.

## See Also

### Creating a URL from a string

init?(string: String)

Creates a URL instance from the provided string.

init?(string: String, relativeTo: URL?)

Creates a URL instance from the provided string, relative to another URL.

init(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Creates a URL that refers to a location specified by resolving bookmark data.

init?(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Initializes a URL that refers to a location specified by resolving bookmark data.

