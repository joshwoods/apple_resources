

- SceneKit
- SCNMaterial
-  shininess 

Instance Property

# shininess

The sharpness of specular highlights. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var shininess: CGFloat { get set }
```

## Discussion

The shininess of a material interacts with its specular property and the lighting in a scene to produce bright highlights on a surface. A higher value produces more sharply defined highlights, making a surface appear more smooth and glossy.

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

var fresnelExponent: CGFloat

A factor affecting the material’s reflectivity. Animatable.

var locksAmbientWithDiffuse: Bool

A Boolean value that determines whether the material responds identically to both ambient and diffuse lighting. Animatable.

