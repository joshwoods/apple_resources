

- Core Foundation
-  CFURLWriteBookmarkDataToFile(\_:\_:\_:\_:) 

Function

# CFURLWriteBookmarkDataToFile(\_:\_:\_:\_:)

Creates an alias file on disk at a specified location with specified bookmark data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLWriteBookmarkDataToFile(
    _ bookmarkRef: CFData!,
    _ fileURL: CFURL!,
    _ options: CFURLBookmarkFileCreationOptions,
    _ errorRef: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`bookmarkRef`  

The bookmark data containing information for the alias file.

`fileURL`  

The desired location of the alias file.

`options`  

Options taken into account when creating the alias file.

`errorRef`  

The error that occurred in the case that the alias file cannot be created.

## Return Value

`true` if the alias file is successfully created; otherwise, `false`.

## See Also

### Working with Bookmark Data

func CFURLCreateBookmarkData(CFAllocator!, CFURL!, CFURLBookmarkCreationOptions, CFArray!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns bookmark data for a URL, created with specified options and resource values.

func CFURLCreateBookmarkDataFromAliasRecord(CFAllocator!, CFData!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from an alias record.

Deprecated

func CFURLCreateBookmarkDataFromFile(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Initializes and returns bookmark data derived from a file pointed to by a specified URL.

func CFURLStartAccessingSecurityScopedResource(CFURL!) -> Bool

In an app that has adopted App Sandbox, makes the resource pointed to by a security-scoped URL available to the app.

func CFURLStopAccessingSecurityScopedResource(CFURL!)

In an app that adopts App Sandbox, revokes access to the resource pointed to by a security-scoped URL.

