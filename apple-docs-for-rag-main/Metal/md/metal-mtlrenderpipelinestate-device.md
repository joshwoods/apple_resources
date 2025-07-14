

- Metal
- MTLRenderPipelineState
-  device 

Instance Property

# device

The device instance that creates the pipeline state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

You can only use the pipeline state object with this device object.

## See Also

### Identifying a Pipeline State

var label: String?

A string that helps you identify the render pipeline state during debugging.

**Required**

var gpuResourceID: MTLResourceID

An unique identifier that represents the pipeline state, which you can add to an argument buffer.

**Required**

