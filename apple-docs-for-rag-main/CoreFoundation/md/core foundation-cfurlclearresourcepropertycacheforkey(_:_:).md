

- Core Foundation
-  CFURLClearResourcePropertyCacheForKey(\_:\_:) 

Function

# CFURLClearResourcePropertyCacheForKey(\_:\_:)

Removes the cached resource value identified by a given key from the URL object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFURLClearResourcePropertyCacheForKey(
    _ url: CFURL!,
    _ key: CFString!
)
```

## Parameters 

`url`  

The URL.

`key`  

The resource value key whose cached values you want to remove.

## Discussion

Removing a cached resource value may remove other cached resource values because some resource values are cached as a set of values, and because some resource values depend on other resource values. (Temporary resource values have no dependencies.)

This method is currently applicable only to URLs for file system resources.

Note

The caching behavior of the `NSURL` and `CFURL` APIs differ. For `NSURL`, all cached values (not temporary values) are automatically removed after each pass through the run loop. You only need to call the CFURL method when you want to clear the cache within a single execution of the run loop. The `CFURL` functions, on the other hand, do not automatically clear cached resource values. The client has complete control over the cache lifetimes, and you must use CFURLClearResourcePropertyCacheForKey(_:_:) or CFURLClearResourcePropertyCache(_:) to clear cached resource values.

## See Also

### Getting and Setting File System Resource Properties

func CFURLClearResourcePropertyCache(CFURL!)

Removes all cached resource values and temporary resource values from the URL object.

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

func CFURLSetResourcePropertyForKey(CFURL!, CFString!, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the URL’s resource property for a given key to a given value.

func CFURLSetTemporaryResourcePropertyForKey(CFURL!, CFString!, CFTypeRef!)

Sets a temporary resource value on the URL.

