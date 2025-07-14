

- Core Foundation
-  CFURLWriteDataAndPropertiesToResource(\_:\_:\_:\_:) Deprecated

Function

# CFURLWriteDataAndPropertiesToResource(\_:\_:\_:\_:)

Writes the given data and properties to a given URL.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFURLWriteDataAndPropertiesToResource(
    _ url: CFURL!,
    _ dataToWrite: CFData!,
    _ propertiesToWrite: CFDictionary!,
    _ errorCode: UnsafeMutablePointer!
) -> Bool
```

Deprecated

For resource data, use the CFWriteStream API. For file resource properties, use CFURLSetResourcePropertiesForKeys.

## Parameters 

`url`  

The resource to write.

`dataToWrite`  

The data to write. Pass `NULL` to write only properties.

`propertiesToWrite`  

The properties to write. Pass `NULL` to write only data. See File URL Properties and HTTP URL Properties for the list of available properties.

`errorCode`  

Upon return, `0` if successful, otherwise contains an error code indicating the nature of the problem. See CFURLError for a list of possible error codes.

## Return Value

`true` if successful, `false` otherwise.

## Discussion

Properties not present in `propertiesToWrite` are left unchanged, hence if `propertiesToWrite` is `NULL` or empty, the URL’s properties are not changed at all.

If `url` uses a file scheme and it references a file, the contents of `dataToWrite` are written to the referenced file, overwriting any preexisting data, and the file’s properties are modified according to `propertiesToWrite`. If the file does not exist, but all intermediate directories along the path do already exist, the file is created (otherwise it is not).

If `url` uses a file scheme and it references a directory (the last path character is “`/`”), the contents of `dataToWrite` are ignored, but if the parameter value is not `NULL`—and all intermediate directories along the path do already exist—a new directory is created (otherwise it is not).

If `url` uses an http scheme, an http `PUT` request is sent to the resource with `propertiesToWrite` as the header fields and `dataToWrite` as the data.

## See Also

### Core Foundation URL Access Utilities Miscellaneous Functions

func CFURLCreateDataAndPropertiesFromResource(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!, CFArray!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Loads the data and properties referred to by a given URL.

Deprecated

func CFURLCreatePropertyFromResource(CFAllocator!, CFURL!, CFString!, UnsafeMutablePointer&lt;Int32>!) -> CFTypeRef!

Returns a given property specified by a given URL and property string.

Deprecated

func CFURLDestroyResource(CFURL!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Destroys a resource indicated by a given URL.

Deprecated

