

- Core Media
-  CMMemoryPoolGetAllocator(\_:) 

Function

# CMMemoryPoolGetAllocator(\_:)

Returns the allocator for the memory pool.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMemoryPoolGetAllocator(_ pool: CMMemoryPool) -> CFAllocator
```

## Parameters 

`pool`  

The memory pool from which to retrieve its allocator.

## Return Value

The memory pool’s allocator.

## See Also

### Managing a Memory Pool

func CMMemoryPoolFlush(CMMemoryPool)

Deallocates all memory the pool holds.

func CMMemoryPoolInvalidate(CMMemoryPool)

Invalidates the memory pool, which causes its allocator to stop recycling memory.

