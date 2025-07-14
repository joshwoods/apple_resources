

- Foundation
- NSURL
-  resourceValues(forKeys:fromBookmarkData:) 

Type Method

# resourceValues(forKeys:fromBookmarkData:)

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func resourceValues(
    forKeys keys: [URLResourceKey],
    fromBookmarkData bookmarkData: Data
) -> [URLResourceKey : Any]?
```

## Parameters 

`keys`  

An array of names of URL resource properties. In addition to the standard, system-defined resource properties, you can also request any custom properties that you provided when you created the bookmark. See the bookmarkData(options:includingResourceValuesForKeys:relativeTo:) method for details.

`bookmarkData`  

The bookmark data from which you want to retrieve resource values.

## Return Value

A dictionary of the requested resource values contained in `bookmarkData`.

## See Also

### Related Documentation

struct URLResourceKey

Keys that apply to file system URLs.

### Working with Bookmark Data

class func bookmarkData(withContentsOf: URL) throws -> Data

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

func bookmarkData(options: NSURL.BookmarkCreationOptions, includingResourceValuesForKeys: [URLResourceKey]?, relativeTo: URL?) throws -> Data

Returns a bookmark for the URL, created with specified options and resource values.

class func writeBookmarkData(Data, to: URL, options: NSURL.BookmarkFileCreationOptions) throws

Creates an alias file on disk at a specified location with specified bookmark data.

func startAccessingSecurityScopedResource() -> Bool

In an app that has adopted App Sandbox, makes the resource pointed to by a security-scoped URL available to the app.

func stopAccessingSecurityScopedResource()

In an app that adopts App Sandbox, revokes access to the resource pointed to by a security-scoped URL.

typealias BookmarkFileCreationOptions

Options used when creating file bookmark data

struct BookmarkCreationOptions

Options used when creating bookmark data.

struct BookmarkResolutionOptions

Options used when resolving bookmark data.

