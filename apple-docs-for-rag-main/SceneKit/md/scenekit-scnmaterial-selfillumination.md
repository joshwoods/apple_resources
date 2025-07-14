

- SceneKit
- SCNMaterial
-  selfIllumination 

Instance Property

# selfIllumination

An object that provides color values representing the global illumination of the surface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var selfIllumination: SCNMaterialProperty { get }
```

## Discussion

Self-illumination applies to all materials, but is especially useful for those using physically-based shading (see physicallyBased). Physically-based materials work best with environment-based lighting (see the SCNScene property lightingEnvironment), but for some materials it can be useful to let a surface itself define part of its lighting—for example, an object whose position obscures it from the “sky” that provides the main lighting environment. When you assign contents to this property, they override the environmental lighting contribution to diffuse shading, but environmental lighting still contributes to specular effects.

## See Also

### Visual Properties for Special Effects

var normal: SCNMaterialProperty

An object that defines the nominal orientation of the surface at each point for use in lighting.

var displacement: SCNMaterialProperty

var emission: SCNMaterialProperty

An object that defines the color emitted by each point on a surface.

var ambientOcclusion: SCNMaterialProperty

An object that provides color values to be multiplied with the ambient light affecting the material.

