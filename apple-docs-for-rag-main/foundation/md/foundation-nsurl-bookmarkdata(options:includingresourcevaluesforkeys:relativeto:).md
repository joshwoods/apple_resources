

- Foundation
- NSURL
-  bookmarkData(options:includingResourceValuesForKeys:relativeTo:) 

Instance Method

# bookmarkData(options:includingResourceValuesForKeys:relativeTo:)

Returns a bookmark for the URL, created with specified options and resource values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func bookmarkData(
    options: NSURL.BookmarkCreationOptions = [],
    includingResourceValuesForKeys keys: [URLResourceKey]?,
    relativeTo relativeURL: URL?
) throws -> Data
```

## Parameters 

`options`  

Options taken into account when creating the bookmark for the URL. The possible flags (which can be combined with bitwise `OR` operations) are described in NSURL.BookmarkCreationOptions.

To create a security-scoped bookmark to support App Sandbox, include the withSecurityScope flag. When you later resolve the bookmark, you can use the resulting security-scoped URL to obtain read/write access to the file-system resource pointed to by the URL.

If you instead want to create a security-scoped bookmark that, when resolved, enables you to obtain read-only access to a file-system resource, bitwise `OR` this parameter’s value with both the withSecurityScope option and the securityScopeAllowOnlyReadAccess option.

`keys`  

An array of names of URL resource properties to store as part of the bookmark. You can later access these values (without resolving the bookmark) by calling the resourceValues(forKeys:fromBookmarkData:) method.

The values of these properties must be of a type that the bookmark generation code can serialize. Specifically, the values can contain any of the following primitive types:

- `NSString` or `CFString`

- `NSData` or `CFData`

- `NSDate` or `CFDate`

- `NSNumber` or `CFNumber`

- `CFBoolean`

- `NSURL` or `CFURL`

- `kCFNull` or NSNull

- `CFUUID`

In addition, the properties can contain the following collection classes:

- `NSArray` or `CFArray` containing only the above primitive types

- `NSDictionary` or `CFDictionary` with `NSString` or `CFString` keys, in which all values contain only the above primitive types

`relativeURL`  

The URL that the bookmark data will be relative to.

If you are creating a security-scoped bookmark to support App Sandbox, use this parameter as follows:

- To create an app-scoped bookmark, use a value of `nil`.

- To create a document-scoped bookmark, use the *absolute* path (despite this parameter’s name) to the document file that is to own the new security-scoped bookmark.

App Sandbox does not restrict which URL values may be passed to this parameter.

## Return Value

A bookmark for the URL.

## Discussion

This method returns bookmark data that can later be resolved into a URL object for a file even if the user moves or renames it (if the volume format on which the file resides supports doing so).

Note

If the specified URL is not a file URL, this method returns a bookmark containing only the URL, and the `options` and `keys` parameters are ignored.

You can also use this method to create a security-scoped bookmark to support App Sandbox. Before you do so, you must first enable the appropriate entitlements for your app, as described in Enabling Security-Scoped Bookmark and URL Access. In addition, be sure to understand the behavior of the `options` and `relativeURL` parameters.

For an app-scoped bookmark, no sandboxed app other than the one that created the bookmark can obtain access to the file-system resource that the URL (obtained from the bookmark) points to. Specifically, a bookmark created with security scope fails to resolve if the caller does not have the same code signing identity as the caller that created the bookmark.

For a document-scoped bookmark, any sandboxed app that has access to the bookmark data itself, and has access to the document that owns the bookmark, can obtain access to the resource.

Version note

Security-scoped bookmarks are not available in versions of macOS prior to OS X v10.7.3.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Working with Bookmark Data

class func bookmarkData(withContentsOf: URL) throws -> Data

Initializes and returns bookmark data derived from an alias file pointed to by a specified URL.

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

