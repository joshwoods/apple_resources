

- Metal
- MTLResource
-  isAliasable() 

Instance Method

# isAliasable()

A Boolean value that indicates whether future heap resource allocations may alias against the resource’s memory.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
func isAliasable() -> Bool
```

**Required**

## Return Value

The default value is false. The value is true only if the makeAliasable() method was previously called on this resource.

## See Also

### Managing Heap Resources

var heapOffset: Int

The distance, in bytes, from the beginning of the heap to the first byte of the resource, if you allocated the resource on a heap.

**Required**

var heap: (any MTLHeap)?

The heap on which the resource is allocated, if any.

**Required**

func makeAliasable()

Allows future heap resource allocations to alias against the resource’s memory, reusing it.

**Required**

