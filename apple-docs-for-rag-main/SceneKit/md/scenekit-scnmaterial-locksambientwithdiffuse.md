

- SceneKit
- SCNMaterial
-  locksAmbientWithDiffuse 

Instance Property

# locksAmbientWithDiffuse

A Boolean value that determines whether the material responds identically to both ambient and diffuse lighting. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var locksAmbientWithDiffuse: Bool { get set }
```

## Discussion

When modeling real-world lighting, a surface is typically considered to have a single “base” color or texture that is visible under both ambient and diffuse light. When this property’s value is false, SceneKit does not have this limitation: you may use a material’s diffuse property to provide a color or texture that is visible under direct lighting, and its ambient property to provide a different color or texture for areas not directly illuminated.

When this property’s value is true, or when using the physicallyBased shading mode, SceneKit uses the diffuse property for ambient lighting, ignoring the ambient property and ensuring that the material responds identically to both ambient and diffuse light.

The default value for this property is true for new apps on all platforms. (In OS X v10.9 and earlier, the default value is false.)

You can animate changes to this property’s value. See Animating SceneKit Content. Animating this property fades between the results of rendering with each state.

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

var fresnelExponent: CGFloat

A factor affecting the material’s reflectivity. Animatable.

