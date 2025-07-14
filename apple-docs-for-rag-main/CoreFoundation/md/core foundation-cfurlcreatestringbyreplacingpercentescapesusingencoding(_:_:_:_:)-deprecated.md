

- Core Foundation
-  CFURLCreateStringByReplacingPercentEscapesUsingEncoding(\_:\_:\_:\_:) Deprecated

Function

# CFURLCreateStringByReplacingPercentEscapesUsingEncoding(\_:\_:\_:\_:)

Creates a new string by replacing any percent escape sequences with their character equivalent.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFURLCreateStringByReplacingPercentEscapesUsingEncoding(
    _ allocator: CFAllocator!,
    _ origString: CFString!,
    _ charsToLeaveEscaped: CFString!,
    _ encoding: CFStringEncoding
) -> CFString!
```

Deprecated

Use \[NSString stringByRemovingPercentEncoding\] or CFURLCreateStringByReplacingPercentEscapes() instead, which always uses the recommended UTF-8 encoding.

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new `CFString` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`origString`  

The `CFString` object to be copied and modified.

`charsToLeaveEscaped`  

Characters whose percent escape sequences, such as `%20` for a space character, you want to leave intact. Pass `NULL` to specify that no percent escapes be replaced, or the empty string (`CFSTR("")`) to specify that all be replaced.

`encoding`  

Specifies the encoding to use when interpreting percent escapes. If you are uncertain of the correct encoding, you should use UTF-8 (CFStringBuiltInEncodings.UTF8), which is the encoding designated by RFC 3986 as the correct encoding for use in URLs.

## Return Value

A new `CFString` object, or `NULL` if the percent escapes cannot be converted to characters, assuming the encoding given by `encoding`. If no characters need to be replaced, this function returns the original string with its reference count incremented. Ownership follows the create rule. See The Create Rule.

## See Also

### Converting URLs to Other Representations

func CFURLCreateData(CFAllocator!, CFURL!, CFStringEncoding, Bool) -> CFData!

Creates a `CFData` object containing the content of a given URL.

func CFURLCreateStringByAddingPercentEscapes(CFAllocator!, CFString!, CFString!, CFString!, CFStringEncoding) -> CFString!

Creates a copy of a string, replacing certain characters with the equivalent percent escape sequence based on the specified encoding.

Deprecated

func CFURLCreateStringByReplacingPercentEscapes(CFAllocator!, CFString!, CFString!) -> CFString!

Creates a new string by replacing any percent escape sequences with their character equivalent.

func CFURLGetFileSystemRepresentation(CFURL!, Bool, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> Bool

Fills a buffer with the file system’s native string representation of a given URL’s path.

func CFURLGetFSRef(CFURL!, OpaquePointer!) -> Bool

Converts a given URL to a file or directory object.

Deprecated

func CFURLGetString(CFURL!) -> CFString!

Returns the URL as a `CFString` object.

