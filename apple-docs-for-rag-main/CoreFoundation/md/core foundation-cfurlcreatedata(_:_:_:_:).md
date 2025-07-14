

- Core Foundation
-  CFURLCreateData(\_:\_:\_:\_:) 

Function

# CFURLCreateData(\_:\_:\_:\_:)

Creates a `CFData` object containing the content of a given URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLCreateData(
    _ allocator: CFAllocator!,
    _ url: CFURL!,
    _ encoding: CFStringEncoding,
    _ escapeWhitespace: Bool
) -> CFData!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new `CFData` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`url`  

The URL to convert into a `CFData` object.

`encoding`  

The string encoding to use when converting `url` into a `CFData` object.

`escapeWhitespace`  

`true` if you want to escape whitespace characters in the URL, `false` otherwise.

## Return Value

A new `CFData` object containing the content of `url`. Ownership follows the create rule. See The Create Rule.

## Discussion

This function escapes any character that is not 7-bit ASCII with the byte-code for the given encoding. If `escapeWhitespace` is `true`, whitespace characters (’ ’, ‘\t’, ‘\r’, ‘\n’) will be escaped as well. This is desirable if you want to embed the URL into a larger text stream like HTML.

## See Also

### Converting URLs to Other Representations

func CFURLCreateStringByAddingPercentEscapes(CFAllocator!, CFString!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a copy of a string, replacing certain characters with the equivalent percent escape sequence based on the specified encoding.

Deprecated

func CFURLCreateStringByReplacingPercentEscapes(CFAllocator!, CFString!, CFString!) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

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

