

- Metal
- MTLRenderPipelineState
-  label 

Instance Property

# label

A string that helps you identify the render pipeline state during debugging.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var label: String? { get }
```

**Required**

## See Also

### Identifying a Pipeline State

var device: any MTLDevice

The device instance that creates the pipeline state.

**Required**

var gpuResourceID: MTLResourceID

An unique identifier that represents the pipeline state, which you can add to an argument buffer.

**Required**

