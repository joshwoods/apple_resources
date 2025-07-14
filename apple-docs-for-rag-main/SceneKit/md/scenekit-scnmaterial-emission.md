

- SceneKit
- SCNMaterial
-  emission 

Instance Property

# emission

An object that defines the color emitted by each point on a surface.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var emission: SCNMaterialProperty { get }
```

## Discussion

You can use an *emissive map* texture to simulate parts of a surface that glow with their own light. SceneKit does not treat the material as a light source—rather, the emission property determines colors for a material independent of lighting. (To create an object that appears to glow, you may wish to combine a geometry with an emissive map and additional SCNLight objects added to the scene.)

By default, the emissive property’s contents object is a black color, causing the property to have no visible effect. Setting the emissive property’s contents to any solid color adds a uniform color to the material independent of lighting. To create a selective glow effect, set the property’s contents to an image or other texture-mapped content whose glowing areas use bright colors and whose other areas use darker colors. In the darker-color portions of the emissive map (and portions with reduced opacity), the other visual properties of the material contribute to its appearance under scene lighting.

The figure below shows a material (with a texture for its diffuse property) before and after providing an emissive map image.

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

var transparent: SCNMaterialProperty

An object that determines the opacity of each point in a material.

### Visual Properties for Special Effects

var normal: SCNMaterialProperty

An object that defines the nominal orientation of the surface at each point for use in lighting.

var displacement: SCNMaterialProperty

var selfIllumination: SCNMaterialProperty

An object that provides color values representing the global illumination of the surface.

var ambientOcclusion: SCNMaterialProperty

An object that provides color values to be multiplied with the ambient light affecting the material.

