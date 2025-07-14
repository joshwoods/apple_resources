

- Core Foundation
-  CFURLCreateDataAndPropertiesFromResource(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# CFURLCreateDataAndPropertiesFromResource(\_:\_:\_:\_:\_:\_:)

Loads the data and properties referred to by a given URL.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFURLCreateDataAndPropertiesFromResource(
    _ alloc: CFAllocator!,
    _ url: CFURL!,
    _ resourceData: UnsafeMutablePointer?>!,
    _ properties: UnsafeMutablePointer?>!,
    _ desiredProperties: CFArray!,
    _ errorCode: UnsafeMutablePointer!
) -> Bool
```

Deprecated

For resource data, use the CFReadStream API. For file resource properties, use CFURLCopyResourcePropertiesForKeys.

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new `CFData` and `CFDictionary` objects returned in `resourceData` and `properties`. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`url`  

The URL referring to the data and/or properties you wish to load.

`resourceData`  

On return, contains a `CFData` object containing the data referred to by `url`. Ownership follows the The Create Rule.

`properties`  

On return, a pointer to a `CFDictionary` object containing the resource properties referred to by `url`. Ownership follows the The Create Rule.

`desiredProperties`  

A list of the properties you wish to obtain and return in `properties`. See File URL Properties and HTTP URL Properties for the list of available properties.

`errorCode`  

`0` if successful, otherwise an error code indicating the nature of the problem. See CFURLError for a list of possible error codes.

## Return Value

`true` if successful, `false` otherwise.

## Discussion

If you are interested in loading only the resource data or the resource’s properties, pass `NULL` for the one you don’t want. If `properties` is non-`NULL` and `desiredProperties` is `NULL` then all properties are fetched. Note that as much work as possible is done even if `false` is returned. For instance, if one property is not available, the others are fetched anyway. This function is intended for convenience, not performance.

## See Also

### Core Foundation URL Access Utilities Miscellaneous Functions

func CFURLCreatePropertyFromResource(CFAllocator!, CFURL!, CFString!, UnsafeMutablePointer&lt;Int32>!) -> CFTypeRef!

Returns a given property specified by a given URL and property string.

Deprecated

func CFURLDestroyResource(CFURL!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Destroys a resource indicated by a given URL.

Deprecated

func CFURLWriteDataAndPropertiesToResource(CFURL!, CFData!, CFDictionary!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Writes the given data and properties to a given URL.

Deprecated

