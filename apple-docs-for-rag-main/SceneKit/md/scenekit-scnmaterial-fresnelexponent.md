

- SceneKit
- SCNMaterial
-  fresnelExponent 

Instance Property

# fresnelExponent

A factor affecting the material’s reflectivity. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var fresnelExponent: CGFloat { get set }
```

## Discussion

The Fresnel exponent of a material interacts with its reflective property to determine the intensity of reflections in a surface based on its angle relative to the viewer. A higher Fresnel exponent increases the visibility of reflections when the material is viewed from a shallow angle.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

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

var transparent: SCNMaterialProperty

An object that determines the opacity of each point in a material.

var shininess: CGFloat

The sharpness of specular highlights. Animatable.

var locksAmbientWithDiffuse: Bool

A Boolean value that determines whether the material responds identically to both ambient and diffuse lighting. Animatable.

