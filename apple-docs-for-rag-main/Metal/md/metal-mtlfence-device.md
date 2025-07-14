

- Metal
- MTLFence
-  device 

Instance Property

# device

The device object that created the fence.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

Only the device that created the fence can use it.

## See Also

### Identifying the Fence

var label: String?

A string that identifies the fence.

**Required**

