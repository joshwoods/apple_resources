

- Core Foundation
-  CFURLCreateBookmarkDataFromAliasRecord(\_:\_:) Deprecated

Function

# CFURLCreateBookmarkDataFromAliasRecord(\_:\_:)

Initializes and returns bookmark data derived from an alias record.

macOS 10.6–11.0Deprecated

``` source
func CFURLCreateBookmarkDataFromAliasRecord(
    _ allocatorRef: CFAllocator!,
    _ aliasRecordDataRef: CFData!
) -> Unmanaged!
```

Deprecated

The Carbon Alias Manager is deprecated. This function should only be used to convert Carbon AliasRecords to bookmark data.

## Parameters 

`allocatorRef`  

The allocator to use to allocate memory for the new `CFURL` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`aliasRecordDataRef`  

The alias record.

## Return Value

The bookmark data for the alias record.

## See Also

### Working with Bookmark Data

func CFURLCreateBookmarkData(CFAllocator!, CFURL!, CFURLBookmarkCreationOptions, CFArray!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns bookmark data for a URL, created with specified options and resource values.

func CFURLCreateBookmarkDataFromFile(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from a file pointed to by a specified URL.

func CFURLWriteBookmarkDataToFile(CFData!, CFURL!, CFURLBookmarkFileCreationOptions, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Creates an alias file on disk at a specified location with specified bookmark data.

func CFURLStartAccessingSecurityScopedResource(CFURL!) -> Bool

In an app that has adopted App Sandbox, makes the resource pointed to by a security-scoped URL available to the app.

func CFURLStopAccessingSecurityScopedResource(CFURL!)

In an app that adopts App Sandbox, revokes access to the resource pointed to by a security-scoped URL.

