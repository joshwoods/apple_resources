

- Foundation
- URL
-  init(resolvingBookmarkData:options:relativeTo:bookmarkDataIsStale:) 

Initializer

# init(resolvingBookmarkData:options:relativeTo:bookmarkDataIsStale:)

Initializes a URL that refers to a location specified by resolving bookmark data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    resolvingBookmarkData data: Data,
    options: URL.BookmarkResolutionOptions = [],
    relativeTo url: URL? = nil,
    bookmarkDataIsStale: inout Bool
) throws
```

## See Also

### Creating a URL from a string

init?(string: String)

Creates a URL instance from the provided string.

init?(string: String, encodingInvalidCharacters: Bool)

Creates a URL instance from the provided string, optionally IDNA- and percent-encoding any invalid characters.

init?(string: String, relativeTo: URL?)

Creates a URL instance from the provided string, relative to another URL.

init(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Creates a URL that refers to a location specified by resolving bookmark data.

