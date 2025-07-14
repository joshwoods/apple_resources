

- Foundation
- URL
-  removeAllCachedResourceValues() 

Instance Method

# removeAllCachedResourceValues()

Removes all cached resource values and all temporary resource values from the URL object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeAllCachedResourceValues()
```

## Discussion

This method is currently applicable only to URLs for file system resources.

## See Also

### Accessing resource values

func resourceValues(forKeys: Set&lt;URLResourceKey>) throws -> URLResourceValues

Returns a collection of resource values identified by the given resource keys.

func setResourceValues(URLResourceValues) throws

Sets the resource value identified by a given resource key.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given resource value key from the URL object.

func setTemporaryResourceValue(any Sendable, forKey: URLResourceKey)

Sets a temporary resource value on the URL object.

struct URLResourceKey

Keys that apply to file system URLs.

struct URLResourceValues

The properties that the file system resources support.

