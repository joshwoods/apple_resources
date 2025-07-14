

- Metal
- MTLResource
-  heap 

Instance Property

# heap

The heap on which the resource is allocated, if any.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var heap: (any MTLHeap)? { get }
```

**Required**

## Discussion

This value is `nil` if the resource isn’t allocated on a heap.

## See Also

### Managing Heap Resources

var heapOffset: Int

The distance, in bytes, from the beginning of the heap to the first byte of the resource, if you allocated the resource on a heap.

**Required**

func makeAliasable()

Allows future heap resource allocations to alias against the resource’s memory, reusing it.

**Required**

func isAliasable() -> Bool

A Boolean value that indicates whether future heap resource allocations may alias against the resource’s memory.

**Required**

