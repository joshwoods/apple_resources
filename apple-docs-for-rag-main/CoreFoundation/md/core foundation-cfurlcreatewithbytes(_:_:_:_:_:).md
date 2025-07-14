

- Core Foundation
-  CFURLCreateWithBytes(\_:\_:\_:\_:\_:) 

Function

# CFURLCreateWithBytes(\_:\_:\_:\_:\_:)

Creates a `CFURL` object using a given character bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLCreateWithBytes(
    _ allocator: CFAllocator!,
    _ URLBytes: UnsafePointer!,
    _ length: CFIndex,
    _ encoding: CFStringEncoding,
    _ baseURL: CFURL!
) -> CFURL!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new `CFURL` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`URLBytes`  

The character bytes to convert into a `CFURL` object.

`length`  

The number of bytes in `URLBytes`.

`encoding`  

The string encoding of the `URLBytes` string. This encoding is also used to interpret percent escape sequences.

`baseURL`  

The URL to which `URLBytes` is relative. Pass `NULL` if `URLBytes` contains an absolute URL or if you want to create a relative URL. If `URLBytes` contains an absolute URL, this parameter is ignored.

## Return Value

A new `CFURL` object. Ownership follows the create rule. See The Create Rule.

## Discussion

The specified string encoding will be used both to interpret `URLBytes`, and to interpret any percent-escapes within the string.

Note

This function does not support string encoding which isn’t a superset of ASCII encoding. Both CFURLGetBytes(_:_:_:) and CFURLGetByteRangeForComponent(_:_:_:) require 7-bit ASCII characters to be stored in a single 8-bit byte. The following CFStringEncodings can be used: CFStringBuiltInEncodings.macRoman, CFStringBuiltInEncodings.windowsLatin1, CFStringBuiltInEncodings.isoLatin1, CFStringBuiltInEncodings.nextStepLatin, CFStringBuiltInEncodings.ASCII and CFStringBuiltInEncodings.UTF8.

## See Also

### Creating a CFURL

func CFURLCopyAbsoluteURL(CFURL!) -> CFURL!

Creates a new `CFURL` object by resolving the relative portion of a URL against its base.

func CFURLCreateAbsoluteURLWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, CFURL!, Bool) -> CFURL!

Creates a new `CFURL` object by resolving the relative portion of a URL, specified as bytes, against its given base URL.

func CFURLCreateByResolvingBookmarkData(CFAllocator!, CFData!, CFURLBookmarkResolutionOptions, CFURL!, CFArray!, UnsafeMutablePointer&lt;DarwinBoolean>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new URL made by resolving bookmark data.

func CFURLCreateCopyAppendingPathComponent(CFAllocator!, CFURL!, CFString!, Bool) -> CFURL!

Creates a copy of a given URL and appends a path component.

func CFURLCreateCopyAppendingPathExtension(CFAllocator!, CFURL!, CFString!) -> CFURL!

Creates a copy of a given URL and appends a path extension.

func CFURLCreateCopyDeletingLastPathComponent(CFAllocator!, CFURL!) -> CFURL!

Creates a copy of a given URL with the last path component deleted.

func CFURLCreateCopyDeletingPathExtension(CFAllocator!, CFURL!) -> CFURL!

Creates a copy of a given URL with its last path extension removed.

func CFURLCreateFilePathURL(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new file path URL that refers to the same resource as a specified URL.

func CFURLCreateFileReferenceURL(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFURL>!

Returns a new file reference URL that points to the same resource as a specified URL.

func CFURLCreateFromFileSystemRepresentation(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, Bool) -> CFURL!

Creates a new `CFURL` object for a file system entity using the native representation.

func CFURLCreateFromFileSystemRepresentationRelativeToBase(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, Bool, CFURL!) -> CFURL!

Creates a `CFURL` object from a native character string path relative to a base URL.

func CFURLCreateFromFSRef(CFAllocator!, OpaquePointer!) -> CFURL!

Creates a URL from a given directory or file.

Deprecated

func CFURLCreateWithFileSystemPath(CFAllocator!, CFString!, CFURLPathStyle, Bool) -> CFURL!

Creates a `CFURL` object using a local file system path string.

func CFURLCreateWithFileSystemPathRelativeToBase(CFAllocator!, CFString!, CFURLPathStyle, Bool, CFURL!) -> CFURL!

Creates a `CFURL` object using a local file system path string relative to a base URL.

func CFURLCreateWithString(CFAllocator!, CFString!, CFURL!) -> CFURL!

Creates a `CFURL` object using a given `CFString` object.

