

- Core Foundation
-  CFURLCreateBookmarkData(\_:\_:\_:\_:\_:\_:) 

Function

# CFURLCreateBookmarkData(\_:\_:\_:\_:\_:\_:)

Returns bookmark data for a URL, created with specified options and resource values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLCreateBookmarkData(
    _ allocator: CFAllocator!,
    _ url: CFURL!,
    _ options: CFURLBookmarkCreationOptions,
    _ resourcePropertiesToInclude: CFArray!,
    _ relativeToURL: CFURL!,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new `CFURL` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`url`  

The URL that bookmark data is being created for.

`options`  

Options taken into account when creating the bookmark data.

To create a security-scoped bookmark to support App Sandbox, include (by way of bitwise `OR` operators with any other options in this parameter) the withSecurityScope option.

When you later resolve the bookmark, you can use the resulting security-scoped URL to obtain read/write access to the file-system resource pointed to by the URL.

If you instead want to create a security-scoped bookmark that, when resolved, enables you to obtain read-only access to a file-system resource, bitwise `OR` this parameter’s value with both the withSecurityScope option and the securityScopeAllowOnlyReadAccess option.

`resourcePropertiesToInclude`  

An array of names of URL resource properties. The values of these properties must be of a type that the bookmark generation code can serialize. Specifically, the values can contain any of the following primitive types:

- `NSString` or `CFString`

- `NSData` or `CFData`

- `NSDate` or `CFDate`

- `NSNumber` or `CFNumber`

- `CFBoolean`

- `NSURL` or `CFURL`

- `CFNull`

- `CFUUID`

In addition, the properties can contain the following collection classes:

- `NSArray` or `CFArray` containing only the above primitive types

- `NSDictionary` or `CFDictionary` with `NSString` or `CFString` keys, in which all values contain only the above primitive types

`relativeToURL`  

The URL that the bookmark data is relative to.

If you are creating a security-scoped bookmark to support App Sandbox, use this parameter as follows:

- To create an app-scoped bookmark, use a value of `nil`.

- To create a document-scoped bookmark, use the *absolute* path (despite this parameter’s name) to the document file that is to own the new security-scoped bookmark.

`error`  

The error that occurred in the case that the bookmark data cannot be created.

## Return Value

The bookmark data for the URL.

## Discussion

To use this function to create a security-scoped bookmark to support App Sandbox, you must first have enabled the appropriate entitlements for your app, as described in Enabling Security-Scoped Bookmark and URL Access. In addition, be sure to understand the behavior of the `options` and `relativeToURL` parameters.

For an app-scoped bookmark, no sandboxed app other than the one that created the bookmark can obtain access to the file-system resource that the URL (obtained from the bookmark) points to. Specifically, a bookmark created with security scope fails to resolve if the caller does not have the same code signing identity as the caller that created the bookmark.

For a document-scoped bookmark, any sandboxed app that has access to the bookmark data itself, and has access to the document that owns the bookmark, can obtain access to the resource.

Version note

Security-scoped bookmarks are not available in versions of macOS prior to OS X v10.7.3.

## See Also

### Related Documentation

func CFURLCreateByResolvingBookmarkData(CFAllocator!, CFData!, CFURLBookmarkResolutionOptions, CFURL!, CFArray!, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new URL made by resolving bookmark data.

### Working with Bookmark Data

func CFURLCreateBookmarkDataFromAliasRecord(CFAllocator!, CFData!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from an alias record.

Deprecated

func CFURLCreateBookmarkDataFromFile(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from a file pointed to by a specified URL.

func CFURLWriteBookmarkDataToFile(CFData!, CFURL!, CFURLBookmarkFileCreationOptions, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Creates an alias file on disk at a specified location with specified bookmark data.

func CFURLStartAccessingSecurityScopedResource(CFURL!) -> Bool

In an app that has adopted App Sandbox, makes the resource pointed to by a security-scoped URL available to the app.

func CFURLStopAccessingSecurityScopedResource(CFURL!)

In an app that adopts App Sandbox, revokes access to the resource pointed to by a security-scoped URL.

