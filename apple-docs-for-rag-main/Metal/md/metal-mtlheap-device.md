

- Metal
- MTLHeap
-  device 

Instance Property

# device

The device object that created the heap.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

A heap is always associated with the MTLDevice that created it and can be used only with that device.

## See Also

### Identifying the Heap

var label: String?

A string that identifies the heap.

**Required**

