

- Foundation
- URL
-  bookmarkData(options:includingResourceValuesForKeys:relativeTo:) 

Instance Method

# bookmarkData(options:includingResourceValuesForKeys:relativeTo:)

Returns bookmark data for the URL, created with specified options and resource values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func bookmarkData(
    options: URL.BookmarkCreationOptions = [],
    includingResourceValuesForKeys keys: Set? = nil,
    relativeTo url: URL? = nil
) throws -> Data
```

## See Also

### Creating bookmarks

static func bookmarkData(withContentsOf: URL) throws -> Data

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

static func writeBookmarkData(Data, to: URL) throws

Creates an alias file on disk at a specified location with specified bookmark data.

static func resourceValues(forKeys: Set&lt;URLResourceKey>, fromBookmarkData: Data) -> URLResourceValues?

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

typealias BookmarkCreationOptions

An alias for bookmark creation options.

struct BookmarkCreationOptions

Options used when creating bookmark data.

