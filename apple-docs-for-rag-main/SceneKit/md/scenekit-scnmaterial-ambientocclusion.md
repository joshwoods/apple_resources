

- SceneKit
- SCNMaterial
-  ambientOcclusion 

Instance Property

# ambientOcclusion

An object that provides color values to be multiplied with the ambient light affecting the material.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var ambientOcclusion: SCNMaterialProperty { get }
```

## Discussion

Use this property to assign an ambient occlusion texture map to a surface. This property has no effect if there is no ambient light in the scene. If this property is not `nil`, SceneKit ignores the ambient property.

When using physically-based shading (see physicallyBased), ambient occlusion approximates large-scale surface details that obscure global illumination.

## See Also

### Visual Properties for Special Effects

var normal: SCNMaterialProperty

An object that defines the nominal orientation of the surface at each point for use in lighting.

var displacement: SCNMaterialProperty

var emission: SCNMaterialProperty

An object that defines the color emitted by each point on a surface.

var selfIllumination: SCNMaterialProperty

An object that provides color values representing the global illumination of the surface.

