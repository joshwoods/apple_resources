

- SceneKit
- SCNMaterial
-  reflective 

Instance Property

# reflective

An object that defines the reflected color for each point on a surface.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var reflective: SCNMaterialProperty { get }
```

## Discussion

You can simulate a mirrored or chromed finish on a surface by causing it to reflect its environment. SceneKit does not render real-time reflections of the objects in a scene, but it can use an *environment map* texture to simulate reflection of a static or animated image. When rendering each pixel on the surface, SceneKit traces the light from that point to a pixel in the environment map as if the surface was reflecting that image.

By default, the reflective property’s contents object is a white color, causing the property to have no visible effect. Setting the reflective property’s contents to any solid color adds uniform shading to the material. To create a reflective effect, set the property’s contents to an image or other texture-mapped content.

To produce a mirror-finish effect using an environment map, the texture image should take one of two forms:

- A sphere map, a square image whose content depicts an environment as reflected by a mirrored sphere.

- A cube map, an array of six square images which together form an imaginary cube enclosing the scene, whose inner surfaces are reflected by the material. You create a cube map by setting the reflective property’s contents object to an NSArray instance containing six images, each corresponding to a direction in the scene’s world coordinate space in the following order: +X, -X, +Y, -Y, +Z, -Z (or Right, Left, Top, Bottom, Near, Far).

The figure below shows a material (with a texture for its normal property) before and after providing a cube map for the reflective property.

This material property does not apply to physically-based materials (see physicallyBased). Instead, such materials reflect environment-based lighting (see the SCNScene lightingEnvironment property) based on their metalness and roughness properties.

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

