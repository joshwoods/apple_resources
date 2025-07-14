

- Foundation
- NSURL
-  writeBookmarkData(\_:to:options:) 

Type Method

# writeBookmarkData(\_:to:options:)

Creates an alias file on disk at a specified location with specified bookmark data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func writeBookmarkData(
    _ bookmarkData: Data,
    to bookmarkFileURL: URL,
    options: NSURL.BookmarkFileCreationOptions
) throws
```

## Parameters 

`bookmarkData`  

The bookmark data containing information for the alias file.

`bookmarkFileURL`  

The desired location of the alias file.

`options`  

Options taken into account when creating the alias file.

## Discussion

This method will produce an error if `bookmarkData` was not created with the `NSURLBookmarkCreationSuitableForBookmarkFile` option.

If `bookmarkFileURL` points to a directory, the alias file will be created in that directory with its name derived from the information in `bookmarkData`. If `bookmarkFileURL` points to a file, the alias file will be created with the location and name indicated by `bookmarkFileURL`, and its extension will be changed to `.alias` if it is not already.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Working with Bookmark Data

class func bookmarkData(withContentsOf: URL) throws -> Data

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

func bookmarkData(options: NSURL.BookmarkCreationOptions, includingResourceValuesForKeys: [URLResourceKey]?, relativeTo: URL?) throws -> Data

Returns a bookmark for the URL, created with specified options and resource values.

class func resourceValues(forKeys: [URLResourceKey], fromBookmarkData: Data) -> [URLResourceKey : Any]?

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

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

