

- Metal
- MTLHeapType
-  MTLHeapType.automatic 

Case

# MTLHeapType.automatic

A heap that automatically places new resource allocations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case automatic
```

## Discussion

In an automatic heap, Metal automatically determines the locations of resources allocated by the heap, with a layout specific to the GPU. Automatic heaps may perform better than manually placing resources in the heap (MTLHeapType.placement).

Use automatic heaps when the heap primarily contains temporary resources that you write to often.

## See Also

### Specifying the Heap Type

case placement

The app controls placement of resources on the heap.

case sparse

The heap contains sparse texture tiles.

