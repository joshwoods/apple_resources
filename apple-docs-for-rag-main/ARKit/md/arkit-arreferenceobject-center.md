

- ARKit
- ARReferenceObject
-  center 

Instance Property

# center

The center point of the reference object’s space-mapping data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var center: simd_float3 { get }
```

## Discussion

The extent and center properties together define a bounding box for the data recorded in the reference object in its local coordinate system. You define that coordinate system with the transform parameter when calling `extractReferenceObject(transform:center:extent:)`, and can modify it by creating another reference object with applyingTransform(_:).

## See Also

### Examining a Reference Object

var name: String?

A descriptive name for the reference object.

var resourceGroupName: String?

var extent: simd_float3

The size of the reference object’s space-mapping data.

var scale: simd_float3

A scale factor for the local coordinate space the reference object defines.

