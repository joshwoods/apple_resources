

- Core Foundation
-  CFURLGetFileSystemRepresentation(\_:\_:\_:\_:) 

Function

# CFURLGetFileSystemRepresentation(\_:\_:\_:\_:)

Fills a buffer with the file system’s native string representation of a given URL’s path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLGetFileSystemRepresentation(
    _ url: CFURL!,
    _ resolveAgainstBase: Bool,
    _ buffer: UnsafeMutablePointer!,
    _ maxBufLen: CFIndex
) -> Bool
```

## Parameters 

`url`  

The `CFURL` object whose native file system representation you want to obtain.

`resolveAgainstBase`  

Pass `true` to return an absolute path name.

`buffer`  

A pointer to a character buffer. On return, the buffer holds the native file system’s representation of `url`. The buffer is null-terminated. This parameter must be at least `maxBufLen` in size for the file system in question to avoid failures for insufficiently large buffers.

`maxBufLen`  

The maximum number of characters that can be written to `buffer`.

## Return Value

`true` if successful, `false` if an error occurred.

## Discussion

No more than `maxBufLen` bytes are written to `buffer`. If `url` requires more than `maxBufLen` bytes to represent itself, including the terminating null byte, this function returns `false`. To avoid this possible failure, you should pass a buffer with size of at least the maximum path length for the file system in question.

## See Also

### Converting URLs to Other Representations

func CFURLCreateData(CFAllocator!, CFURL!, CFStringEncoding, Bool) -> CFData!

Creates a `CFData` object containing the content of a given URL.

func CFURLCreateStringByAddingPercentEscapes(CFAllocator!, CFString!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a copy of a string, replacing certain characters with the equivalent percent escape sequence based on the specified encoding.

Deprecated

func CFURLCreateStringByReplacingPercentEscapes(CFAllocator!, CFString!, CFString!) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

func CFURLCreateStringByReplacingPercentEscapesUsingEncoding(CFAllocator!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

Deprecated

func CFURLGetFSRef(CFURL!, OpaquePointer!) -> Bool

Converts a given URL to a file or directory object.

Deprecated

func CFURLGetString(CFURL!) -> CFString!

Returns the URL as a `CFString` object.

