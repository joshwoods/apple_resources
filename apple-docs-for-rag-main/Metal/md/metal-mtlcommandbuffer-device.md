

- Metal
- MTLCommandBuffer
-  device 

Instance Property

# device

The GPU device that indirectly owns the command buffer because you create it from a command queue the device also owns.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

The command buffer can only work with other instances that device creates, directly or indirectly, such as buffers and textures.

## See Also

### Identifying the Command Buffer

var label: String?

An optional name that can help you identify the command buffer.

**Required**

var commandQueue: any MTLCommandQueue

The command queue that creates the command buffer.

**Required**

