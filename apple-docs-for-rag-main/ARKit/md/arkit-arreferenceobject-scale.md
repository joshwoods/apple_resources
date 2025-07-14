

- ARKit
- ARReferenceObject
-  scale 

Instance Property

# scale

A scale factor for the local coordinate space the reference object defines.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var scale: simd_float3 { get }
```

## Discussion

Multiplying the extent by this scale results in the physical size of the object in meters.

## See Also

### Examining a Reference Object

var name: String?

A descriptive name for the reference object.

var resourceGroupName: String?

var center: simd_float3

The center point of the reference object’s space-mapping data.

var extent: simd_float3

The size of the reference object’s space-mapping data.

