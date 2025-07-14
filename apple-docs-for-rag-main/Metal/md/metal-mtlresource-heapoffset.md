

- Metal
- MTLResource
-  heapOffset 

Instance Property

# heapOffset

The distance, in bytes, from the beginning of the heap to the first byte of the resource, if you allocated the resource on a heap.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var heapOffset: Int { get }
```

**Required**

## Discussion

If the heap is not a placement heap (MTLHeapType.placement), the value is always `0` and should be ignored.

## See Also

### Managing Heap Resources

var heap: (any MTLHeap)?

The heap on which the resource is allocated, if any.

**Required**

func makeAliasable()

Allows future heap resource allocations to alias against the resource’s memory, reusing it.

**Required**

func isAliasable() -> Bool

A Boolean value that indicates whether future heap resource allocations may alias against the resource’s memory.

**Required**

