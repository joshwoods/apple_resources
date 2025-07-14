

- Foundation
- URL
-  URL.BookmarkResolutionOptions 

Type Alias

# URL.BookmarkResolutionOptions

An alias for the bookmark resolution options type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias BookmarkResolutionOptions = NSURL.BookmarkResolutionOptions
```

## See Also

### Creating a URL by resolving a bookmark

init(resolvingBookmarkData: Data, options: URL.BookmarkResolutionOptions, relativeTo: URL?, bookmarkDataIsStale: inout Bool) throws

Creates a URL that refers to a location specified by resolving bookmark data.

init(resolvingAliasFileAt: URL, options: URL.BookmarkResolutionOptions) throws

Creates a URL that refers to the location specified by resolving an alias file.

struct BookmarkResolutionOptions

Options used when resolving bookmark data.

