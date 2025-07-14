

- Core Foundation
-  CFURLCreatePropertyFromResource(\_:\_:\_:\_:) Deprecated

Function

# CFURLCreatePropertyFromResource(\_:\_:\_:\_:)

Returns a given property specified by a given URL and property string.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func CFURLCreatePropertyFromResource(
    _ alloc: CFAllocator!,
    _ url: CFURL!,
    _ property: CFString!,
    _ errorCode: UnsafeMutablePointer!
) -> CFTypeRef!
```

Deprecated

For file resource properties, use CFURLCopyResourcePropertyForKey.

## Parameters 

`alloc`  

The allocator to use to to allocate memory for the new `CFType` object for the requested property. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`url`  

The `CFURL` object referring to the resource whose properties are loaded.

`property`  

The name of the property you wish to load. Pass one of the provided string constants indicating the property. See File URL Properties and HTTP URL Properties for the list of available properties.

`errorCode`  

On return, `0` if successful, otherwise an error code indicating the nature of the problem. See CFURLError for a list of possible error codes.

## Return Value

If successful, the requested property as a `CFType` object, `NULL` otherwise. Ownership follows the The Create Rule.

## Discussion

This is a convenience function for retrieving individual property values which calls through to CFURLCreateDataAndPropertiesFromResource(_:_:_:_:_:_:).

## See Also

### Core Foundation URL Access Utilities Miscellaneous Functions

func CFURLCreateDataAndPropertiesFromResource(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!, CFArray!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Loads the data and properties referred to by a given URL.

Deprecated

func CFURLDestroyResource(CFURL!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Destroys a resource indicated by a given URL.

Deprecated

func CFURLWriteDataAndPropertiesToResource(CFURL!, CFData!, CFDictionary!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Writes the given data and properties to a given URL.

Deprecated

