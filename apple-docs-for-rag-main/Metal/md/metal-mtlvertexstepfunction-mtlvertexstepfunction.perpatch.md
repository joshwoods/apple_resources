

- Metal
- MTLVertexStepFunction
-  MTLVertexStepFunction.perPatch 

Case

# MTLVertexStepFunction.perPatch

The post-tessellation vertex function fetches data based on the patch index of the patch.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
case perPatch
```

## See Also

### Constants

case constant

The vertex function fetches attribute data once and uses that data for every vertex.

case perVertex

The vertex function fetches and uses new attribute data for every vertex.

case perInstance

The vertex function regularly fetches new attribute data for a number of instances that is determined by `stepRate`.

case perPatchControlPoint

The post-tessellation vertex function fetches data based on the control-point indices associated with the patch.

