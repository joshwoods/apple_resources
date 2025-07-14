

- Foundation
- URL
-  resourceValues(forKeys:fromBookmarkData:) 

Type Method

# resourceValues(forKeys:fromBookmarkData:)

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func resourceValues(
    forKeys keys: Set,
    fromBookmarkData data: Data
) -> URLResourceValues?
```

## Discussion

If the result dictionary does not contain a resource value for one or more of the requested resource keys, it means those resource properties are not available in the bookmark data.

## See Also

### Creating bookmarks

func bookmarkData(options: URL.BookmarkCreationOptions, includingResourceValuesForKeys: Set&lt;URLResourceKey>?, relativeTo: URL?) throws -> Data

Returns bookmark data for the URL, created with specified options and resource values.

static func bookmarkData(withContentsOf: URL) throws -> Data

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

static func writeBookmarkData(Data, to: URL) throws

Creates an alias file on disk at a specified location with specified bookmark data.

typealias BookmarkCreationOptions

An alias for bookmark creation options.

struct BookmarkCreationOptions

Options used when creating bookmark data.

