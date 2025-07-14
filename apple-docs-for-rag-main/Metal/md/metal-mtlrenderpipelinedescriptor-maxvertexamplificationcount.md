

- Metal
- MTLRenderPipelineDescriptor
-  maxVertexAmplificationCount 

Instance Property

# maxVertexAmplificationCount

The maximum vertex amplification count you can set when encoding render commands.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var maxVertexAmplificationCount: Int { get set }
```

## Mentioned in 

Improving Rendering Performance with Vertex Amplification

## Discussion

Before setting this property, call the supportsVertexAmplificationCount(_:) method on the device object to determine whether that amplification count is supported.

## See Also

### Related Documentation

func setVertexAmplificationCount(Int, viewMappings: UnsafePointer&lt;MTLVertexAmplificationViewMapping>?)

Configures the number of output vertices the render pipeline produces for each input vertex, optionally with render target and viewport offsets.

**Required**

func supportsVertexAmplificationCount(Int) -> Bool

Returns a Boolean value that indicates whether the GPU supports an amplification factor.

**Required**

