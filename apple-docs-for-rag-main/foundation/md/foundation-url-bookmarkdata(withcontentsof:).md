

- Foundation
- URL
-  bookmarkData(withContentsOf:) 

Type Method

# bookmarkData(withContentsOf:)

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func bookmarkData(withContentsOf url: URL) throws -> Data
```

## Discussion

If bookmarkFileURL refers to an alias file created prior to OS X 10.6 that contains Alias Manager information but no bookmark data, this method synthesizes bookmark data for the file.

## See Also

### Creating bookmarks

func bookmarkData(options: URL.BookmarkCreationOptions, includingResourceValuesForKeys: Set&lt;URLResourceKey>?, relativeTo: URL?) throws -> Data

Returns bookmark data for the URL, created with specified options and resource values.

static func writeBookmarkData(Data, to: URL) throws

Creates an alias file on disk at a specified location with specified bookmark data.

static func resourceValues(forKeys: Set&lt;URLResourceKey>, fromBookmarkData: Data) -> URLResourceValues?

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

typealias BookmarkCreationOptions

An alias for bookmark creation options.

struct BookmarkCreationOptions

Options used when creating bookmark data.

