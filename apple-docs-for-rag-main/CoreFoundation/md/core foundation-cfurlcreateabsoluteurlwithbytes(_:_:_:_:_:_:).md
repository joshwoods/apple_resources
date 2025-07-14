

- Core Foundation
-  CFURLCreateAbsoluteURLWithBytes(\_:\_:\_:\_:\_:\_:) 

Function

# CFURLCreateAbsoluteURLWithBytes(\_:\_:\_:\_:\_:\_:)

Creates a new `CFURL` object by resolving the relative portion of a URL, specified as bytes, against its given base URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLCreateAbsoluteURLWithBytes(
    _ alloc: CFAllocator!,
    _ relativeURLBytes: UnsafePointer!,
    _ length: CFIndex,
    _ encoding: CFStringEncoding,
    _ baseURL: CFURL!,
    _ useCompatibilityMode: Bool
) -> CFURL!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new `CFURL` object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`relativeURLBytes`  

The character bytes that represent a relative URL to convert into a `CFURL` object.

`length`  

The number of bytes in `relativeURLBytes`.

`encoding`  

The string encoding of the `relativeURLBytes` string. This encoding is also used to interpret percent escape sequences.

`baseURL`  

The URL to which `relativeURLBytes` is relative.

`useCompatibilityMode`  

If `true`, the rules historically used on the web are used to resolve the string specified by the `relativeURLBytes` parameter against `baseURL`. These rules are generally listed in the RFC as optional or alternate interpretations. Otherwise, the strict rules from the RFC are used.

## Return Value

A new `CFURL` object, or `NULL` if `relativeURLBytes` cannot be made absolute. Ownership follows the create rule. See The Create Rule.

## Discussion

This function interprets the provided bytes using the specified string encoding to create the relative portion of the URL’s address.

Note

This function does not support string encoding which isn’t a superset of ASCII encoding. Both CFURLGetBytes(_:_:_:) and CFURLGetByteRangeForComponent(_:_:_:) require 7-bit ASCII characters to be stored in a single 8-bit byte. The following CFStringEncodings can be used: CFStringBuiltInEncodings.macRoman, CFStringBuiltInEncodings.windowsLatin1, CFStringBuiltInEncodings.isoLatin1, CFStringBuiltInEncodings.nextStepLatin, CFStringBuiltInEncodings.ASCII and CFStringBuiltInEncodings.UTF8.

## See Also

### Creating a CFURL

func CFURLCopyAbsoluteURL(CFURL!) -> CFURL!

Creates a new `CFURL` object by resolving the relative portion of a URL against its base.

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

func CFURLCreateWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, CFURL!) -> CFURL!

Creates a `CFURL` object using a given character bytes.

func CFURLCreateWithFileSystemPath(CFAllocator!, CFString!, CFURLPathStyle, Bool) -> CFURL!

Creates a `CFURL` object using a local file system path string.

func CFURLCreateWithFileSystemPathRelativeToBase(CFAllocator!, CFString!, CFURLPathStyle, Bool, CFURL!) -> CFURL!

Creates a `CFURL` object using a local file system path string relative to a base URL.

func CFURLCreateWithString(CFAllocator!, CFString!, CFURL!) -> CFURL!

Creates a `CFURL` object using a given `CFString` object.

