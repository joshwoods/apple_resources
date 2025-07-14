

- Metal
- MTLCommandQueue
-  device 

Instance Property

# device

The GPU device that creates the command queue.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

The command queue can submit work only to the GPU the MTLDevice instance represents.

## See Also

### Identifying the Command Queue

var label: String?

An optional name that can help you identify the command queue.

**Required**

