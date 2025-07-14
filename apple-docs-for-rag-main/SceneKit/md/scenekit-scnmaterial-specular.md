

- SceneKit
- SCNMaterial
-  specular 

Instance Property

# specular

An object that manages the material’s specular response to lighting.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var specular: SCNMaterialProperty { get }
```

## Discussion

Specular shading describes the amount and color of light reflected by the material directly toward the viewer, forming a bright highlight on the surface and simulating a glossy or shiny appearance. You adjust the sharpness of specular highlights using the material’s shininess property.

By default, the specular property’s contents object is a black color, causing the material to appear dull or matte. Changing the specular property’s contents to a brighter color causes specular highlights to appear in that color, making the surface appear shiny. When you apply a texture to the specular property, the texture image becomes a *specular map*—the brightness of each pixel in the image determines the tendency of each point on the material’s surface to create specular highlights when lit.

The figure below shows a material (with a texture for its diffuse property) before and after providing a specular map image. Notice that the bright specular highlights appear only on portions of the surface where the specular map image is white.

The material’s lightingModel property determines the formula SceneKit uses to combine its specularity and other visual properties with lights and other contents in a scene to produce the final color for each rendered pixel in the rendered scene. For details, see `Lighting Models`.

This material property does not apply to physically-based materials (see physicallyBased).

## See Also

### Related Documentation

var normal: SCNMaterialProperty

An object that defines the nominal orientation of the surface at each point for use in lighting.

var emission: SCNMaterialProperty

An object that defines the color emitted by each point on a surface.

### Visual Properties for Basic Shading

var diffuse: SCNMaterialProperty

An object that manages the material’s diffuse response to lighting.

var ambient: SCNMaterialProperty

An object that manages the material’s response to ambient lighting.

var reflective: SCNMaterialProperty

An object that defines the reflected color for each point on a surface.

var multiply: SCNMaterialProperty

An object that provides color values that are multiplied with pixels in a material after all other shading is complete.

var transparent: SCNMaterialProperty

An object that determines the opacity of each point in a material.

var shininess: CGFloat

The sharpness of specular highlights. Animatable.

var fresnelExponent: CGFloat

A factor affecting the material’s reflectivity. Animatable.

var locksAmbientWithDiffuse: Bool

A Boolean value that determines whether the material responds identically to both ambient and diffuse lighting. Animatable.

