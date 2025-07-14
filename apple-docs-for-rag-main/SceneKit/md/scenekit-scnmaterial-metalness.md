

- SceneKit
- SCNMaterial
-  metalness 

Instance Property

# metalness

An object that provides color values to determine how metallic the material’s surface appears.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var metalness: SCNMaterialProperty { get }
```

## Discussion

This property measures only the total intensity of color values; texture contents are best defined in grayscale.

This property generally approximates aspects of a physical surface—such as index of refraction, tendency to produce sharp reflections, and tendency to produce Fresnel reflections at grazing angles—that together produce an overall metallic or nonmetallic (also called dielectric) appearance. Lower values (darker colors) cause the material to appear more like a dielectric surface. Higher values (brighter colors) cause the surface to appear more metallic.

This property applies only when the material’s lightingModel value is physicallyBased.

## See Also

### Visual Properties for Physically Based Shading

var diffuse: SCNMaterialProperty

An object that manages the material’s diffuse response to lighting.

var roughness: SCNMaterialProperty

An object that provides color values to determine the apparent smoothness of the surface.

