

- Core Foundation
-  CFURLDestroyResource(\_:\_:) Deprecated

Function

# CFURLDestroyResource(\_:\_:)

Destroys a resource indicated by a given URL.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFURLDestroyResource(
    _ url: CFURL!,
    _ errorCode: UnsafeMutablePointer!
) -> Bool
```

Deprecated

Use CFURLGetFileSystemRepresentation and removefile(3) instead.

## Parameters 

`url`  

The `CFURL` object of the resource to destroy.

`errorCode`  

On return, `0` if successful, otherwise an error code indicating the nature of the problem. See CFURLError for a list of possible error codes.

## Return Value

`true` if successful, `false` otherwise.

## Discussion

If `url` uses an http scheme, an http `DELETE` request is sent to the resource. If `url` uses a file scheme, then:

- if the reference is a file, the file is deleted;

- if the reference is a directory and the directory is empty, the directory is deleted;

- if the reference is a directory and the directory is not empty, the function returns `false` and `errorCode` contains `kCFURLUnknownError`.

## See Also

### Core Foundation URL Access Utilities Miscellaneous Functions

func CFURLCreateDataAndPropertiesFromResource(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!, CFArray!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Loads the data and properties referred to by a given URL.

Deprecated

func CFURLCreatePropertyFromResource(CFAllocator!, CFURL!, CFString!, UnsafeMutablePointer&lt;Int32>!) -> CFTypeRef!

Returns a given property specified by a given URL and property string.

Deprecated

func CFURLWriteDataAndPropertiesToResource(CFURL!, CFData!, CFDictionary!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Writes the given data and properties to a given URL.

Deprecated

