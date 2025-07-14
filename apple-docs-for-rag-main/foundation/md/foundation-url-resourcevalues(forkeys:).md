

- Foundation
- URL
-  resourceValues(forKeys:) 

Instance Method

# resourceValues(forKeys:)

Returns a collection of resource values identified by the given resource keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func resourceValues(forKeys keys: Set) throws -> URLResourceValues
```

## Parameters 

`keys`  

A set of URL resource keys indicating the values to retrieve.

## Return Value

A URLResourceValues instance, containing the retrieved values.

## Discussion

This method first checks if the URL instance already caches the specified resource values. If so, it returns the cached resource values to the caller. If not, then this method synchronously obtains the resource values from the backing store, adds them to the URL object’s cache, and returns a populated URLResourceValues instance. This method only populates URLResourceValues members corresponding to the contents of the `keys` parameter.

The type of the returned resource value varies by resource property; for details, see the documentation for the URLResourceKey you want to access.

If there’s no available value for a given key in `keys`, the returned URLResourceValues contains `nil` for the corresponding item. If this method fails to determine a value’s availability or retrieve its value, the method throws an error.

When you call this method from the main thread, the URL removes cached resource values the next time the thread’s run loop runs, except those added as temporary properties. You can explicitly remove cached resource values with removeCachedResourceValue(forKey:) and removeAllCachedResourceValues().

Note

This method is currently applicable only to URLs for file system resources.

## See Also

### Accessing resource values

func setResourceValues(URLResourceValues) throws

Sets the resource value identified by a given resource key.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given resource value key from the URL object.

func removeAllCachedResourceValues()

Removes all cached resource values and all temporary resource values from the URL object.

func setTemporaryResourceValue(any Sendable, forKey: URLResourceKey)

Sets a temporary resource value on the URL object.

struct URLResourceKey

Keys that apply to file system URLs.

struct URLResourceValues

The properties that the file system resources support.

