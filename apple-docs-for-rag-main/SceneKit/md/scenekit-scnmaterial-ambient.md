

- SceneKit
- SCNMaterial
-  ambient 

Instance Property

# ambient

An object that manages the material’s response to ambient lighting.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var ambient: SCNMaterialProperty { get }
```

## Discussion

Ambient shading describes the amount and color of ambient light reflected by the material. Ambient shading is uniform in all directions at all points on a surface. If a scene does not contain lights whose type is ambient, this property has no effect on a material’s appearance.

By default, the ambient property’s contents object is a dark gray color. Changing the ambient property’s contents lets you specify a different color or texture for the areas of a surface not directly illuminated by lights in a scene. To make the material respond identically to both ambient and diffuse light, set its locksAmbientWithDiffuse property to true.

The figure below shows a material (with a texture for its diffuse property) before and after setting the ambient property’s contents to a solid color.

The material’s lightingModel property determines the formula SceneKit uses to combine its ambient color and other visual properties with lights and other contents in a scene to produce the final color for each rendered pixel in the rendered scene. For details, see `Lighting Models`.

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

var specular: SCNMaterialProperty

An object that manages the material’s specular response to lighting.

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

