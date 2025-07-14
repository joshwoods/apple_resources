

- Foundation
- URLCache
-  init(memoryCapacity:diskCapacity:diskPath:) 

Initializer

# init(memoryCapacity:diskCapacity:diskPath:)

Creates a URL cache object with the specified values.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
init(
    memoryCapacity: Int,
    diskCapacity: Int,
    diskPath path: String?
)
```

## Parameters 

`memoryCapacity`  

The memory capacity of the cache, in bytes.

`diskCapacity`  

The disk capacity of the cache, in bytes.

`path`  

In macOS, `path` is the location at which to store the on-disk cache.

In iOS, `path` is the name of a subdirectory of the application’s default cache directory in which to store the on-disk cache (the subdirectory is created if it does not exist).

## Return Value

The initialized cache object.

## Discussion

The returned cache instance is backed by disk, so you have more leeway when choosing the capacity for this kind of cache. A disk cache measured in the tens of megabytes should be acceptable in most cases.

## See Also

### Related Documentation

class var shared: URLCache

The shared URL cache instance.

### Creating a new cache object

convenience init(memoryCapacity: Int, diskCapacity: Int, directory: URL?)

Creates a URL cache object with the specified memory and disk capacities, in the specified directory.

