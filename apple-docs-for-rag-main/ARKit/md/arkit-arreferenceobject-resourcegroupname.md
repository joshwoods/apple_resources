

- ARKit
- ARReferenceObject
-  resourceGroupName 

Instance Property

# resourceGroupName

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var resourceGroupName: String? { get }
```

## Discussion

If ARKit loaded this object from an AR resource group in an asset catalog, ARKit sets the value of this property to the resource group’s name. Otherwise, the value of this property is `nil`.

## See Also

### Examining a Reference Object

var name: String?

A descriptive name for the reference object.

var center: simd_float3

The center point of the reference object’s space-mapping data.

var extent: simd_float3

The size of the reference object’s space-mapping data.

var scale: simd_float3

A scale factor for the local coordinate space the reference object defines.

