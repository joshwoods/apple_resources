

- Metal
- MTLVertexAmplificationViewMapping
-  renderTargetArrayIndexOffset 

Instance Property

# renderTargetArrayIndexOffset

An offset into the list of render targets.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var renderTargetArrayIndexOffset: UInt32
```

## Mentioned in 

Improving Rendering Performance with Vertex Amplification

## Discussion

To specify a list of offsets, call the setVertexAmplificationCount(_:viewMappings:) method.

When your app renders to different render targets, you specify the render target index to render to in your vertex shader by adding the `render_target_array_index` attribute to one of the vertex shader’s outputs. If you are using vertex amplification, Metal calculates the index for each amplified vertex by adding the index offset for the vertex to the value returned from your shader.

## See Also

### Specifying Mapping Offsets

var viewportArrayIndexOffset: UInt32

An offset into the list of viewports.

