

- SceneKit
- SCNMaterial
-  multiply 

Instance Property

# multiply

An object that provides color values that are multiplied with pixels in a material after all other shading is complete.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var multiply: SCNMaterialProperty { get }
```

## Discussion

After combining a material’s other visual properties with lighting and other information about a scene, Scene kit multiplies the color of each rendered pixel by the color this property provides. You can use this property to darken or tint a surface independent of the effects of lighting and other properties, or to add precomputed lighting to a scene via a shadow map.

By default, the multiply property’s contents object is a white color, causing the property to have no visible effect.

The figure below shows a material (with textures for its diffuse and emission properties) before and after setting the multiply property’s contents to a solid color. Notice that the multiply color modulates even the bright areas added by the emissive map.

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

var specular: SCNMaterialProperty

An object that manages the material’s specular response to lighting.

var reflective: SCNMaterialProperty

An object that defines the reflected color for each point on a surface.

var transparent: SCNMaterialProperty

An object that determines the opacity of each point in a material.

var shininess: CGFloat

The sharpness of specular highlights. Animatable.

var fresnelExponent: CGFloat

A factor affecting the material’s reflectivity. Animatable.

var locksAmbientWithDiffuse: Bool

A Boolean value that determines whether the material responds identically to both ambient and diffuse lighting. Animatable.

