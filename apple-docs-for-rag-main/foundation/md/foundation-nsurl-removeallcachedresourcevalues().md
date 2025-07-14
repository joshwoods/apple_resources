

- Foundation
- NSURL
-  removeAllCachedResourceValues() 

Instance Method

# removeAllCachedResourceValues()

Removes all cached resource values and temporary resource values from the URL object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeAllCachedResourceValues()
```

## Discussion

This method is applicable only to URLs that represent file system resources.

Note

The caching behavior of the `NSURL` and `CFURL` APIs differ. For `NSURL`, all cached values (not temporary values) are automatically removed after each pass through the run loop. You only need to call the removeCachedResourceValue(forKey:) method when you want to clear the cache within a single execution of the run loop. The `CFURL` functions, on the other hand, do not automatically clear cached resource values. The client has complete control over the cache lifetimes, and you must use CFURLClearResourcePropertyCacheForKey(_:_:) or CFURLClearResourcePropertyCache(_:) to clear cached resource values.

## See Also

### Accessing Resource Values

func resourceValues(forKeys: [URLResourceKey]) throws -> [URLResourceKey : Any]

Returns the resource values for the properties identified by specified array of keys.

func getResourceValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, forKey: URLResourceKey) throws

Returns the value of the resource property for the specified key.

func setResourceValue(Any?, forKey: URLResourceKey) throws

Sets the URL’s resource property for a given key to a given value.

func setResourceValues([URLResourceKey : Any]) throws

Sets the URL’s resource properties for a given set of keys to a given set of values.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given key from the URL object.

func setTemporaryResourceValue((any Sendable)?, forKey: URLResourceKey)

Sets a temporary resource value on the URL object.

struct URLResourceKey

Keys that apply to file system URLs.

