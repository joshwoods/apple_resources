

- Metal
- MTLDevice
-  areBarycentricCoordsSupported Deprecated

Instance Property

# areBarycentricCoordsSupported

A Boolean value that indicates whether the GPU supports barycentric coordinates.

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOS 10.15–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var areBarycentricCoordsSupported: Bool { get }
```

**Required**

Deprecated

Use supportsShaderBarycentricCoordinates instead.

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

func supportsVertexAmplificationCount(Int) -> Bool

Returns a Boolean value that indicates whether the GPU supports an amplification factor.

**Required**

var areProgrammableSamplePositionsSupported: Bool

A Boolean value that indicates whether the GPU supports programmable sample positions.

**Required**

var areRasterOrderGroupsSupported: Bool

A Boolean value that indicates whether the GPU supports raster order groups.

**Required**

