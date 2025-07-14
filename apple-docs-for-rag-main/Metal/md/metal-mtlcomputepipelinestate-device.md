

- Metal
- MTLComputePipelineState
-  device 

Instance Property

# device

The device instance that created the pipeline state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

This compute state instance is only usable on the device set in this property.

## See Also

### Identifying a Pipeline State

var gpuResourceID: MTLResourceID

An unique identifier that represents the pipeline state, which you can add to an argument buffer.

**Required**

var label: String?

A string that helps you identify the compute pipeline state during debugging.

**Required**

