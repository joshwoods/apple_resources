

- Core Foundation
-  CFURLCreateBookmarkDataFromFile(\_:\_:\_:) 

Function

# CFURLCreateBookmarkDataFromFile(\_:\_:\_:)

Initializes and returns bookmark data derived from a file pointed to by a specified URL.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLCreateBookmarkDataFromFile(
    _ allocator: CFAllocator!,
    _ fileURL: CFURL!,
    _ errorRef: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new `CFURL` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`fileURL`  

The file URL.

`errorRef`  

The error that occurred in the case that the bookmark data cannot be created.

## Return Value

The bookmark data for the file, or `NULL` if an error occurs.

## See Also

### Working with Bookmark Data

func CFURLCreateBookmarkData(CFAllocator!, CFURL!, CFURLBookmarkCreationOptions, CFArray!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns bookmark data for a URL, created with specified options and resource values.

func CFURLCreateBookmarkDataFromAliasRecord(CFAllocator!, CFData!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from an alias record.

Deprecated

func CFURLWriteBookmarkDataToFile(CFData!, CFURL!, CFURLBookmarkFileCreationOptions, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Creates an alias file on disk at a specified location with specified bookmark data.

func CFURLStartAccessingSecurityScopedResource(CFURL!) -> Bool

In an app that has adopted App Sandbox, makes the resource pointed to by a security-scoped URL available to the app.

func CFURLStopAccessingSecurityScopedResource(CFURL!)

In an app that adopts App Sandbox, revokes access to the resource pointed to by a security-scoped URL.

