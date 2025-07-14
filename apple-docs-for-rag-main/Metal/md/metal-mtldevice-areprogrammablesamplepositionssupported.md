

- Metal
- MTLDevice
-  areProgrammableSamplePositionsSupported 

Instance Property

# areProgrammableSamplePositionsSupported

A Boolean value that indicates whether the GPU supports programmable sample positions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var areProgrammableSamplePositionsSupported: Bool { get }
```

**Required**

## Mentioned in 

Positioning Samples Programmatically

Storing Data a Pass Makes with Custom Sample Positions for a Subsequent Pass

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

var areRasterOrderGroupsSupported: Bool

A Boolean value that indicates whether the GPU supports raster order groups.

**Required**

var areBarycentricCoordsSupported: Bool

A Boolean value that indicates whether the GPU supports barycentric coordinates.

**Required**

Deprecated

