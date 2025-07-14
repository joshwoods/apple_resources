

- SceneKit
- SCNMaterial
-  transparent 

Instance Property

# transparent

An object that determines the opacity of each point in a material.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var transparent: SCNMaterialProperty { get }
```

## Discussion

Use this property to selectively make parts of a material appear transparent. You can uniformly adjust the opacity of a material using its transparency property, or of all the content attached to a node using the node’s opacity property.

By default, the transparent property’s contents object is a fully opaque black color, causing the property to have no visible effect. Setting the transparent property’s contents to any solid color uniformly fades the opacity of the material based on that color’s opacity value. To make parts of a material appear transparent, set the property’s contents to an image or other texture-mapped content whose alpha channel defines areas of full or partial opacity.

The figure below shows a semitransparent material before and after providing a texture image for its transparent property. (To make the transparency effect more visible, a blue sphere is shown behind the transparent material.)

The transparencyMode property controls how SceneKit interprets color information from the transparent property’s contents.

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

var multiply: SCNMaterialProperty

An object that provides color values that are multiplied with pixels in a material after all other shading is complete.

var shininess: CGFloat

The sharpness of specular highlights. Animatable.

var fresnelExponent: CGFloat

A factor affecting the material’s reflectivity. Animatable.

var locksAmbientWithDiffuse: Bool

A Boolean value that determines whether the material responds identically to both ambient and diffuse lighting. Animatable.

