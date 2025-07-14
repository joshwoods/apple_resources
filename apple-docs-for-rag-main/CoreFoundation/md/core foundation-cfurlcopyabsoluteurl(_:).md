

- Core Foundation
-  CFURLCopyAbsoluteURL(\_:) 

Function

# CFURLCopyAbsoluteURL(\_:)

Creates a new `CFURL` object by resolving the relative portion of a URL against its base.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFURLCopyAbsoluteURL(_ relativeURL: CFURL!) -> CFURL!
```

## Parameters 

`relativeURL`  

The `CFURL` object to resolve.

## Return Value

A new `CFURL` object, or `NULL` if `relativeURL` cannot be made absolute. Ownership follows the create rule. See The Create Rule.

## See Also

### Creating a CFURL

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

func CFURLCreateWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, CFURL!) -> CFURL!

Creates a `CFURL` object using a given character bytes.

func CFURLCreateWithFileSystemPath(CFAllocator!, CFString!, CFURLPathStyle, Bool) -> CFURL!

Creates a `CFURL` object using a local file system path string.

func CFURLCreateWithFileSystemPathRelativeToBase(CFAllocator!, CFString!, CFURLPathStyle, Bool, CFURL!) -> CFURL!

Creates a `CFURL` object using a local file system path string relative to a base URL.

func CFURLCreateWithString(CFAllocator!, CFString!, CFURL!) -> CFURL!

Creates a `CFURL` object using a given `CFString` object.

