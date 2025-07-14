

- Core Foundation
-  CFURLStopAccessingSecurityScopedResource(\_:) 

Function

# CFURLStopAccessingSecurityScopedResource(\_:)

In an app that adopts App Sandbox, revokes access to the resource pointed to by a security-scoped URL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLStopAccessingSecurityScopedResource(_ url: CFURL!)
```

## Parameters 

`url`  

The security-scoped URL that points to the file-system resource you want to stop accessing.

## Discussion

When you no longer need access to a file or directory pointed to by a security-scoped URL, such as one returned by resolving a security-scoped bookmark, call this function (or its Cocoa equivalent, stopAccessingSecurityScopedResource()) on the URL.

Warning

You must balance every call to the CFURLStartAccessingSecurityScopedResource(_:) method with a corresponding call to the CFURLStopAccessingSecurityScopedResource(_:) method. If you fail to relinquish your access when you no longer need a file-system resource, your app leaks kernel resources. If sufficient kernel resources are leaked, your app loses its ability to add file-system locations to its sandbox, such as via Powerbox or security-scoped bookmarks, until relaunched.

Version note

Security-scoped bookmarks are not available in versions of macOS prior to OS X v10.7.3.

## See Also

### Working with Bookmark Data

func CFURLCreateBookmarkData(CFAllocator!, CFURL!, CFURLBookmarkCreationOptions, CFArray!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns bookmark data for a URL, created with specified options and resource values.

func CFURLCreateBookmarkDataFromAliasRecord(CFAllocator!, CFData!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from an alias record.

Deprecated

func CFURLCreateBookmarkDataFromFile(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from a file pointed to by a specified URL.

func CFURLWriteBookmarkDataToFile(CFData!, CFURL!, CFURLBookmarkFileCreationOptions, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Creates an alias file on disk at a specified location with specified bookmark data.

func CFURLStartAccessingSecurityScopedResource(CFURL!) -> Bool

In an app that has adopted App Sandbox, makes the resource pointed to by a security-scoped URL available to the app.

