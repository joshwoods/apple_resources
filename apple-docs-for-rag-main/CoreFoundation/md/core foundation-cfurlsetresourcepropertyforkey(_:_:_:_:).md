

- Core Foundation
-  CFURLSetResourcePropertyForKey(\_:\_:\_:\_:) 

Function

# CFURLSetResourcePropertyForKey(\_:\_:\_:\_:)

Sets the URL’s resource property for a given key to a given value.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLSetResourcePropertyForKey(
    _ url: CFURL!,
    _ key: CFString!,
    _ propertyValue: CFTypeRef!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

## Parameters 

`url`  

The URL.

`key`  

The name of one of the URL’s resource properties.

`propertyValue`  

The value for the resource property defined by `key`.

`error`  

The error that occurred if the resource value could not be set.

## Return Value

`true` if the resource property named `key` is successfully set to `value`; otherwise, `false`.

## Discussion

This function synchronously writes the new resource value out to disk. Attempts to set a read-only resource property or to set a resource property that is not supported by the resource are ignored and are not considered errors.

If an error occurs, this method returns `false` and populates the object pointer referenced by `error` with additional information.

Note

This method applies only to URLs for file system resources.

## See Also

### Related Documentation

class CFURL

### Getting and Setting File System Resource Properties

func CFURLClearResourcePropertyCache(CFURL!)

Removes all cached resource values and temporary resource values from the URL object.

func CFURLClearResourcePropertyCacheForKey(CFURL!, CFString!)

Removes the cached resource value identified by a given key from the URL object.

func CFURLCopyResourcePropertiesForKeys(CFURL!, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFDictionary>!

Returns the resource values for the properties identified by specified array of keys.

func CFURLCopyResourcePropertyForKey(CFURL!, CFString!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Returns the value of a given resource property of a given URL.

func CFURLCreateResourcePropertiesForKeysFromBookmarkData(CFAllocator!, CFArray!, CFData!) -> Unmanaged&lt;CFDictionary>!

Returns the resource values for properties identified by a specified array of keys contained in specified bookmark data.

func CFURLCreateResourcePropertyForKeyFromBookmarkData(CFAllocator!, CFString!, CFData!) -> Unmanaged&lt;CFTypeRef>!

Returns the value of a resource property from specified bookmark data.

func CFURLSetResourcePropertiesForKeys(CFURL!, CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the URL’s resource properties for a given set of keys to a given set of values.

func CFURLSetTemporaryResourcePropertyForKey(CFURL!, CFString!, CFTypeRef!)

Sets a temporary resource value on the URL.

