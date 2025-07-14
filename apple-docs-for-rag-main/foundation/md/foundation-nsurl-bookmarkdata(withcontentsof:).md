

- Foundation
- NSURL
-  bookmarkData(withContentsOf:) 

Type Method

# bookmarkData(withContentsOf:)

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func bookmarkData(withContentsOf bookmarkFileURL: URL) throws -> Data
```

## Parameters 

`bookmarkFileURL`  

The URL that points to a file containing bookmark data.

## Return Value

The bookmark data for the alias file.

## Discussion

This method doesn’t check to see if `bookmarkFileURL` points to an alias file. This allows this method to work with any file containing bookmark data. If `bookmarkFileURL` refers to a file which does not contain bookmark data or to a non-file object, such as a directory or symbolic link, this method returns `nil` produces an error.

This method returns `nil` if bookmark data cannot be created.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Working with Bookmark Data

func bookmarkData(options: NSURL.BookmarkCreationOptions, includingResourceValuesForKeys: [URLResourceKey]?, relativeTo: URL?) throws -> Data

Returns a bookmark for the URL, created with specified options and resource values.

class func resourceValues(forKeys: [URLResourceKey], fromBookmarkData: Data) -> [URLResourceKey : Any]?

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

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

