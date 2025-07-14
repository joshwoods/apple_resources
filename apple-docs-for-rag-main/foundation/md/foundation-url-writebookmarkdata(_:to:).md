

- Foundation
- URL
-  writeBookmarkData(\_:to:) 

Type Method

# writeBookmarkData(\_:to:)

Creates an alias file on disk at a specified location with specified bookmark data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func writeBookmarkData(
    _ data: Data,
    to url: URL
) throws
```

## Discussion

The `data` must have been created with the suitableForBookmarkFile option. The `url` must either refer to an existing file (which will be overwritten), or to location in an existing directory.

## See Also

### Creating bookmarks

func bookmarkData(options: URL.BookmarkCreationOptions, includingResourceValuesForKeys: Set&lt;URLResourceKey>?, relativeTo: URL?) throws -> Data

Returns bookmark data for the URL, created with specified options and resource values.

static func bookmarkData(withContentsOf: URL) throws -> Data

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

static func resourceValues(forKeys: Set&lt;URLResourceKey>, fromBookmarkData: Data) -> URLResourceValues?

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

typealias BookmarkCreationOptions

An alias for bookmark creation options.

struct BookmarkCreationOptions

Options used when creating bookmark data.

