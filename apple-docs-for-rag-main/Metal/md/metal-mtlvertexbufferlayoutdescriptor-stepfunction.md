

- Metal
- MTLVertexBufferLayoutDescriptor
-  stepFunction 

Instance Property

# stepFunction

The circumstances under which the vertex and its attributes are presented to the vertex function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var stepFunction: MTLVertexStepFunction { get set }
```

## Discussion

The default value is MTLVertexStepFunction.perVertex.

If `stepFunction` is MTLVertexStepFunction.perVertex, the function fetches new attribute data based on the `[[ vertex_id ]]` attribute qualifier. The function fetches new attribute data each time a new vertex is processed. In this case, `stepRate` must be set to `1`, which is its default value.

If `stepFunction` is MTLVertexStepFunction.perInstance, the function fetches new attribute data based on the `[[ instance_id ]]` attribute qualifier. In this case, `stepRate` must be greater than `0` and its value determines how often the function fetches new attribute data.

If `stepFunction` is MTLVertexStepFunction.constant, the function fetches attribute data just once, and that attribute data is used for every vertex. In this case,`stepRate` must be set to `0`.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Organizing the Vertex Buffer Layout

var stepRate: Int

The interval at which the vertex and its attributes are presented to the vertex function.

var stride: Int

The number of bytes between the first byte of two consecutive vertices in a buffer.

