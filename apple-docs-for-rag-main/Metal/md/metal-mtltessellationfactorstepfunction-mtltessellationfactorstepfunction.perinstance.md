

- Metal
- MTLTessellationFactorStepFunction
-  MTLTessellationFactorStepFunction.perInstance 

Case

# MTLTessellationFactorStepFunction.perInstance

A per-instance step function. For a given instance ID, the tessellation factor for a patch in a patch draw call is at the `offset + (instanceID * instanceStride)` location in the tessellation factor buffer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
case perInstance
```

## See Also

### Constants

case constant

A constant step function. For all instances, the tessellation factor for all patches in a patch draw call is at the `offset` location in the tessellation factor buffer.

case perPatch

A per-patch step function. For all instances, the tessellation factor for all patches in a patch draw call is at the `offset + (drawPatchIndex * tessellationFactorStride)` location in the tessellation factor buffer.

case perPatchAndPerInstance

A per-patch and per-instance step function. For a given instance ID, the tessellation factor for a patch in a patch draw call is at the `offset + (drawPatchIndex * tessellationFactorStride + instanceID * instanceStride)` location in the tessellation factor buffer.

