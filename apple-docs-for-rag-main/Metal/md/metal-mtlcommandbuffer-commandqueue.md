

- Metal
- MTLCommandBuffer
-  commandQueue 

Instance Property

# commandQueue

The command queue that creates the command buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var commandQueue: any MTLCommandQueue { get }
```

**Required**

## Discussion

Each command buffer can only submit its commands to the queue that creates it.

## See Also

### Identifying the Command Buffer

var label: String?

An optional name that can help you identify the command buffer.

**Required**

var device: any MTLDevice

The GPU device that indirectly owns the command buffer because you create it from a command queue the device also owns.

**Required**

