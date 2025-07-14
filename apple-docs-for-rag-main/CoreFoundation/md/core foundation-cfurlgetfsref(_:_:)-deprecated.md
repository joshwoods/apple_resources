

- Core Foundation
-  CFURLGetFSRef(\_:\_:) Deprecated

Function

# CFURLGetFSRef(\_:\_:)

Converts a given URL to a file or directory object.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFURLGetFSRef(
    _ url: CFURL!,
    _ fsRef: OpaquePointer!
) -> Bool
```

Deprecated

Not supported

## Parameters 

`url`  

The `CFURL` object to convert to a file or directory object.

`fsRef`  

Upon return, contains the file or directory object representing `url`.

## Return Value

`true` if the conversion was successful, otherwise `false`.

## Discussion

The function cannot create an `FSRef` object if any of the leading path parts specified by `url` is an alias. The function can, however, traverse symbolic links.

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

func CFURLGetFileSystemRepresentation(CFURL!, Bool, UnsafeMutablePointer&lt;UInt8>!, CFIndex) -> Bool

Fills a buffer with the file system’s native string representation of a given URL’s path.

func CFURLGetString(CFURL!) -> CFString!

Returns the URL as a `CFString` object.

