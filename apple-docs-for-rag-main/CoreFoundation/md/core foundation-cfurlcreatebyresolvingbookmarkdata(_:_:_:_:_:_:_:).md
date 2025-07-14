

- Core Foundation
-  CFURLCreateByResolvingBookmarkData(\_:\_:\_:\_:\_:\_:\_:) 

Function

# CFURLCreateByResolvingBookmarkData(\_:\_:\_:\_:\_:\_:\_:)

Returns a new URL made by resolving bookmark data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLCreateByResolvingBookmarkData(
    _ allocator: CFAllocator!,
    _ bookmark: CFData!,
    _ options: CFURLBookmarkResolutionOptions,
    _ relativeToURL: CFURL!,
    _ resourcePropertiesToInclude: CFArray!,
    _ isStale: UnsafeMutablePointer!,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new `CFURL` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bookmark`  

The bookmark data the URL is derived from.

`options`  

Options taken into account when resolving the bookmark data.

To resolve a security-scoped bookmark to support App Sandbox, you must include (by way of bitwise `OR` operators with any other options in this parameter) the cfurlBookmarkResolutionWithSecurityScope option.

`relativeToURL`  

The base URL that the bookmark data is relative to. Can be `NULL`.

If you are resolving a security-scoped bookmark to obtain a security-scoped URL, use this parameter as follows:

- To resolve an app-scoped bookmark, use a value of `nil`.

- To resolve a document-scoped bookmark, use the *absolute* path (despite this parameter’s name) to the document from which you retrieved the bookmark.

`resourcePropertiesToInclude`  

An array of resource properties to include when creating the URL. Can be `NULL`.

`isStale`  

If true, the bookmark data is stale.

`error`  

The error that occurred in the case that the URL cannot be created.

## Return Value

A new URL made by resolving `bookmark`, or `NULL` if an error occurs.

## Discussion

To obtain a security-scoped URL from a security-scoped bookmark, call this method using the cfurlBookmarkResolutionWithSecurityScope option. In addition, to use security scope, you must first have enabled the appropriate entitlements for your app, as described in Enabling Security-Scoped Bookmark and URL Access.

To then obtain access to the file-system resource pointed to by a security-scoped URL (in other words, to bring the resource into your app’s sandbox), call the CFURLStartAccessingSecurityScopedResource(_:) function (or its Cocoa equivalent) on the URL.

For an app-scoped bookmark, no sandboxed app other than the one that created the bookmark can obtain access to the file-system resource that the URL (obtained from the bookmark) points to.

For a document-scoped bookmark, any sandboxed app that has access to the bookmark data itself, and has access to the document that owns the bookmark, can obtain access to the resource.

Version note

Security-scoped bookmarks are not available in versions of macOS prior to OS X v10.7.3.

## See Also

### Related Documentation

func CFURLCreateBookmarkData(CFAllocator!, CFURL!, CFURLBookmarkCreationOptions, CFArray!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns bookmark data for a URL, created with specified options and resource values.

### Creating a CFURL

func CFURLCopyAbsoluteURL(CFURL!) -> CFURL!

Creates a new `CFURL` object by resolving the relative portion of a URL against its base.

func CFURLCreateAbsoluteURLWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, CFURL!, Bool) -> CFURL!

Creates a new `CFURL` object by resolving the relative portion of a URL, specified as bytes, against its given base URL.

func CFURLCreateCopyAppendingPathComponent(CFAllocator!, CFURL!, CFString!, Bool) -> CFURL!

Creates a copy of a given URL and appends a path component.

func CFURLCreateCopyAppendingPathExtension(CFAllocator!, CFURL!, CFString!) -> CFURL!

Creates a copy of a given URL and appends a path extension.

func CFURLCreateCopyDeletingLastPathComponent(CFAllocator!, CFURL!) -> CFURL!

Creates a copy of a given URL with the last path component deleted.

func CFURLCreateCopyDeletingPathExtension(CFAllocator!, CFURL!) -> CFURL!

Creates a copy of a given URL with its last path extension removed.

func CFURLCreateFilePathURL(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new file path URL that refers to the same resource as a specified URL.

func CFURLCreateFileReferenceURL(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new file reference URL that points to the same resource as a specified URL.

func CFURLCreateFromFileSystemRepresentation(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, Bool) -> CFURL!

Creates a new `CFURL` object for a file system entity using the native representation.

func CFURLCreateFromFileSystemRepresentationRelativeToBase(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, Bool, CFURL!) -> CFURL!

Creates a `CFURL` object from a native character string path relative to a base URL.

func CFURLCreateFromFSRef(CFAllocator!, OpaquePointer!) -> CFURL!

Creates a URL from a given directory or file.

Deprecated

func CFURLCreateWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, CFURL!) -> CFURL!

Creates a `CFURL` object using a given character bytes.

func CFURLCreateWithFileSystemPath(CFAllocator!, CFString!, CFURLPathStyle, Bool) -> CFURL!

Creates a `CFURL` object using a local file system path string.

func CFURLCreateWithFileSystemPathRelativeToBase(CFAllocator!, CFString!, CFURLPathStyle, Bool, CFURL!) -> CFURL!

Creates a `CFURL` object using a local file system path string relative to a base URL.

func CFURLCreateWithString(CFAllocator!, CFString!, CFURL!) -> CFURL!

Creates a `CFURL` object using a given `CFString` object.

