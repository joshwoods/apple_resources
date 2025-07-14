

- Core Foundation
-  CFURLCreateStringByReplacingPercentEscapes(\_:\_:\_:) 

Function

# CFURLCreateStringByReplacingPercentEscapes(\_:\_:\_:)

Creates a new string by replacing any percent escape sequences with their character equivalent.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLCreateStringByReplacingPercentEscapes(
    _ allocator: CFAllocator!,
    _ originalString: CFString!,
    _ charactersToLeaveEscaped: CFString!
) -> CFString!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new `CFString` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`originalString`  

The `CFString` object to be copied and modified.

`charactersToLeaveEscaped`  

Characters whose percent escape sequences, such as `%20` for a space character, you want to leave intact. Pass `NULL` to specify that no percent escapes be replaced, or the empty string (`CFSTR("")`) to specify that all be replaced.

## Return Value

A new `CFString` object, or `NULL` if the percent escapes cannot be converted to characters, assuming UTF-8 encoding. If no characters need to be replaced, this function returns the original string with its reference count incremented. Ownership follows the create rule. See The Create Rule.

## See Also

### Converting URLs to Other Representations

func CFURLCreateData(CFAllocator!, CFURL!, CFStringEncoding, Bool) -> CFData!

Creates a `CFData` object containing the content of a given URL.

func CFURLCreateStringByAddingPercentEscapes(CFAllocator!, CFString!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a copy of a string, replacing certain characters with the equivalent percent escape sequence based on the specified encoding.

Deprecated

func CFURLCreateStringByReplacingPercentEscapesUsingEncoding(CFAllocator!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

Deprecated

func CFURLGetFileSystemRepresentation(CFURL!, Bool, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> Bool

Fills a buffer with the file system’s native string representation of a given URL’s path.

func CFURLGetFSRef(CFURL!, OpaquePointer!) -> Bool

Converts a given URL to a file or directory object.

Deprecated

func CFURLGetString(CFURL!) -> CFString!

Returns the URL as a `CFString` object.

