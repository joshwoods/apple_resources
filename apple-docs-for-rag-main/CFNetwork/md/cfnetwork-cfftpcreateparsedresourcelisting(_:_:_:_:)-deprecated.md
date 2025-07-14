

- CFNetwork
-  CFFTPCreateParsedResourceListing(\_:\_:\_:\_:) Deprecated

Function

# CFFTPCreateParsedResourceListing(\_:\_:\_:\_:)

Parses an FTP listing to a dictionary.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.3–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func CFFTPCreateParsedResourceListing(
    _ alloc: CFAllocator?,
    _ buffer: UnsafePointer,
    _ bufferLength: CFIndex,
    _ parsed: UnsafeMutablePointer?>?
) -> CFIndex
```

Deprecated

Use NSURLSessionAPI for ftp requests

## Parameters 

`alloc`  

The allocator to use to allocate memory for the dictionary. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`buffer`  

A pointer to a buffer holding zero or more lines of resource listing.

`bufferLength`  

The length in bytes of the buffer pointed to by `buffer`.

`parsed`  

Upon return, contains a dictionary containing the parsed resource information. If parsing fails, a `NULL` pointer is returned.

## Return Value

The number of bytes parsed, `0` if no bytes were available for parsing, or `-1` if parsing failed.

## Discussion

This function examines the contents of buffer as an FTP directory listing and parses into a CFDictionary the information for a single file or folder. The CFDictionary is returned in the `parsed` parameter, and the number of bytes used from buffer is returned.

## See Also

### FTP

let kCFFTPResourceGroup: CFString

CFDictionary key for getting the CFString containing the name of a group that shares the FTP resource.

Deprecated

let kCFFTPResourceLink: CFString

CFDictionary key for getting the CFString containing the symbolic link information. If the item is a symbolic link, the CFString contains the path to the item that the link references.

Deprecated

let kCFFTPResourceModDate: CFString

CFDictionary key for getting the CFDate containing the last date and time the FTP resource was modified.

Deprecated

let kCFFTPResourceMode: CFString

CFDictionary key for getting the CFNumber containing the access permissions, defined in `sys/types.h`, of the FTP resource.

Deprecated

let kCFFTPResourceName: CFString

CFDictionary key for getting the CFString containing the name of the FTP resource.

Deprecated

let kCFFTPResourceOwner: CFString

CFDictionary key for getting the CFString containing the name of the owner of the FTP resource.

Deprecated

let kCFFTPResourceSize: CFString

CFDictionary key for getting the CFNumber containing the size in bytes of the FTP resource.

Deprecated

let kCFFTPResourceType: CFString

CFDictionary key for getting the CFNumber containing the type of the FTP resource as defined in `sys/dirent.h`.

Deprecated

