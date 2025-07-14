

- Metal
- MTLHeapType
-  MTLHeapType.placement 

Case

# MTLHeapType.placement

The app controls placement of resources on the heap.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case placement
```

## Discussion

Use placement heaps when you need direct control over memory use and heap fragmentation. Typically, you use placement heaps for resources you keep for long time periods and rarely change.

## See Also

### Specifying the Heap Type

case automatic

A heap that automatically places new resource allocations.

case sparse

The heap contains sparse texture tiles.

