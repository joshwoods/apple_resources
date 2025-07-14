

- Metal
- MTLDevice
-  supportsVertexAmplificationCount(\_:) 

Instance Method

# supportsVertexAmplificationCount(\_:)

Returns a Boolean value that indicates whether the GPU supports an amplification factor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
func supportsVertexAmplificationCount(_ count: Int) -> Bool
```

**Required**

## Parameters 

`count`  

An integer that represents the number of output streams you want the GPU to generate from an input stream.

## Mentioned in 

Improving Rendering Performance with Vertex Amplification

## Discussion

A vertex amplification factor of `1` has no effect because it effectively disables vertex amplification.

Important

Passing a vertex amplification factor of `1` or less to this method triggers an API validation error.

For more information about vertex amplification, see Improving Rendering Performance with Vertex Amplification.

## See Also

### Checking Render Support

var supportsRaytracing: Bool

A Boolean value that indicates whether the GPU device supports ray tracing.

**Required**

var supportsPrimitiveMotionBlur: Bool

A Boolean value that indicates whether the GPU device supports motion blur for ray tracing.

**Required**

var supportsRaytracingFromRender: Bool

A Boolean value that indicates whether you can call ray-tracing functions from a vertex or fragment shader.

**Required**

var supports32BitMSAA: Bool

A Boolean value that indicates whether the GPU can allocate 32-bit integer texture formats and resolve to 32-bit floating-point texture formats.

**Required**

var supportsPullModelInterpolation: Bool

A Boolean value that indicates whether the GPU can compute multiple interpolations of a fragment function’s input.

**Required**

var supportsShaderBarycentricCoordinates: Bool

A Boolean value that indicates whether the GPU supports barycentric coordinates.

**Required**

var areProgrammableSamplePositionsSupported: Bool

A Boolean value that indicates whether the GPU supports programmable sample positions.

**Required**

var areRasterOrderGroupsSupported: Bool

A Boolean value that indicates whether the GPU supports raster order groups.

**Required**

var areBarycentricCoordsSupported: Bool

A Boolean value that indicates whether the GPU supports barycentric coordinates.

**Required**

Deprecated

