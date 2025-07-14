

- Foundation
- URLCache
-  init(memoryCapacity:diskCapacity:directory:) 

Initializer

# init(memoryCapacity:diskCapacity:directory:)

Creates a URL cache object with the specified memory and disk capacities, in the specified directory.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(
    memoryCapacity: Int,
    diskCapacity: Int,
    directory: URL? = nil
)
```

## Parameters 

`memoryCapacity`  

The memory capacity of the cache, in bytes.

`diskCapacity`  

The disk capacity of the cache, in bytes.

`directory`  

The path to an on-disk directory, where the system stores the on-disk cache. If `directory` is `nil`, the cache uses a default directory.

## Discussion

A disk cache measured in the tens of megabytes is acceptable in most cases.

## See Also

### Creating a new cache object

init(memoryCapacity: Int, diskCapacity: Int, diskPath: String?)

Creates a URL cache object with the specified values.

