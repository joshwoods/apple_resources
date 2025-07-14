

- Metal
- MTLDevice
-  supportsPrimitiveMotionBlur 

Instance Property

# supportsPrimitiveMotionBlur

A Boolean value that indicates whether the GPU device supports motion blur for ray tracing.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var supportsPrimitiveMotionBlur: Bool { get }
```

**Required**

## See Also

### Checking Render Support

var supportsRaytracing: Bool

A Boolean value that indicates whether the GPU device supports ray tracing.

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

func supportsVertexAmplificationCount(Int) -> Bool

Returns a Boolean value that indicates whether the GPU supports an amplification factor.

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

