

- Core Media
-  CMMemoryPoolInvalidate(\_:) 

Function

# CMMemoryPoolInvalidate(\_:)

Invalidates the memory pool, which causes its allocator to stop recycling memory.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMemoryPoolInvalidate(_ pool: CMMemoryPool)
```

## Parameters 

`pool`  

The memory pool to invalidate.

## See Also

### Managing a Memory Pool

func CMMemoryPoolGetAllocator(CMMemoryPool) -> CFAllocator

Returns the allocator for the memory pool.

func CMMemoryPoolFlush(CMMemoryPool)

Deallocates all memory the pool holds.

