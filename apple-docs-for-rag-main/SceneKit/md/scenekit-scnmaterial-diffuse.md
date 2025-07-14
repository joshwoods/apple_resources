

- SceneKit
- SCNMaterial
-  diffuse 

Instance Property

# diffuse

An object that manages the material’s diffuse response to lighting.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var diffuse: SCNMaterialProperty { get }
```

## Discussion

Diffuse shading describes the amount and color of light reflected equally in all directions from each point on the material’s surface. The diffuse color of a pixel is independent of the point of view, so it can be thought of as a material’s “base” color or texture.

By default, the diffuse property’s contents object is a white color. The figure below shows the effect of setting the diffuse property’s contents to a texture image on a material whose other properties have default contents.

The material’s lightingModel property determines the formula SceneKit uses to combine its diffuse color and other visual properties with lights and other contents in a scene to produce the final color for each rendered pixel in the rendered scene. For details, see `Lighting Models`.

## See Also

### Related Documentation

var specular: SCNMaterialProperty

An object that manages the material’s specular response to lighting.

var reflective: SCNMaterialProperty

An object that defines the reflected color for each point on a surface.

var multiply: SCNMaterialProperty

An object that provides color values that are multiplied with pixels in a material after all other shading is complete.

var ambient: SCNMaterialProperty

An object that manages the material’s response to ambient lighting.

var normal: SCNMaterialProperty

An object that defines the nominal orientation of the surface at each point for use in lighting.

var emission: SCNMaterialProperty

An object that defines the color emitted by each point on a surface.

var transparent: SCNMaterialProperty

An object that determines the opacity of each point in a material.

### Visual Properties for Physically Based Shading

var metalness: SCNMaterialProperty

An object that provides color values to determine how metallic the material’s surface appears.

var roughness: SCNMaterialProperty

An object that provides color values to determine the apparent smoothness of the surface.

