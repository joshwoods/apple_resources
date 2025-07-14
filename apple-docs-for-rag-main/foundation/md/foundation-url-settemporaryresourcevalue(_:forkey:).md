

- Foundation
- URL
-  setTemporaryResourceValue(\_:forKey:) 

Instance Method

# setTemporaryResourceValue(\_:forKey:)

Sets a temporary resource value on the URL object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@preconcurrency
mutating func setTemporaryResourceValue(
    _ value: any Sendable,
    forKey key: URLResourceKey
)
```

## Discussion

Temporary resource values are for client use. Temporary resource values exist only in memory and are never written to the resource’s backing store. Once set, a temporary resource value can be copied from the URL object with `func resourceValues(forKeys:)`. The values are stored in the loosely-typed `allValues` dictionary property.

To remove a temporary resource value from the URL object, use `func removeCachedResourceValue(forKey:)`. Care should be taken to ensure the key that identifies a temporary resource value is unique and does not conflict with system defined keys (using reverse domain name notation in your temporary resource value keys is recommended). This method is currently applicable only to URLs for file system resources.

## See Also

### Accessing resource values

func resourceValues(forKeys: Set&lt;URLResourceKey>) throws -> URLResourceValues

Returns a collection of resource values identified by the given resource keys.

func setResourceValues(URLResourceValues) throws

Sets the resource value identified by a given resource key.

func removeCachedResourceValue(forKey: URLResourceKey)

Removes the cached resource value identified by a given resource value key from the URL object.

func removeAllCachedResourceValues()

Removes all cached resource values and all temporary resource values from the URL object.

struct URLResourceKey

Keys that apply to file system URLs.

struct URLResourceValues

The properties that the file system resources support.

