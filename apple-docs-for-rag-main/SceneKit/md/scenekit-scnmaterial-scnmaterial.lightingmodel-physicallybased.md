

- SceneKit
- SCNMaterial
- SCNMaterial.LightingModel
-  physicallyBased 

Type Property

# physicallyBased

Shading based on a realistic abstraction of physical lights and materials.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let physicallyBased: SCNMaterial.LightingModel
```

## Discussion

Physically-based shading incorporates a refined model of the interactions between real-world lights and materials. Using modern GPU hardware and algorithms, this model can produce more realistic results than the loose abstractions of traditional shading, while also offering a set of material properties that is easier for artists to work with. Especially when combined with environmental lighting (see the SCNScene lightingEnvironment property) and high dynamic range cameras (see the SCNCamera wantsHDR property), physically-based shading can produce realistic results similar to those seen in recent animated feature films.

Physically based shading relies primarily on three material properties:

- The diffuse property (called albedo in some authoring tools) provides the “base” color of a material.

- The roughness property (inverted and called smoothness in some authoring tools) is an approximation of the microscopic detail in a real-world surface. By approximating these “microfacets” as a single term, this property helps produce lighting calculations that resemble the energy-conserving laws of real-world physics, resulting in more realistic variation between matte and shiny surfaces.

- The metalness property approximates other aspects of a physical surface, such as index of refraction, tendency to produce sharp reflections, and tendency to produce Fresnel reflections at grazing angles, which together produce an overall metallic or nonmetallic (also called dielectric) appearance.

In addition, you can add surface detail to a physically based material with the normal and ambientOcclusion properties, and modulate the contribution of environmental lighting with the selfIllumination property.

Physically based materials ignore the ambient, specular, and reflective material properties and the shininess, fresnelExponent, and locksAmbientWithDiffuse parameters.

Note

Physically based rendering requires a Metal renderer. When displaying a material in a view whose renderingAPI value is not SCNRenderingAPI.metal, SceneKit falls back to rendering that material with the blinn lighting model. (Metal rendering is not supported in Simulator or Xcode Playgrounds when targeting iOS or tvOS, and is not available at all in watchOS, so this fallback always occurs in those environments.)

## See Also

### Type Properties

static let blinn: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Blinn-Phong formula.

static let constant: SCNMaterial.LightingModel

Uniform shading that incorporates ambient lighting only.

static let lambert: SCNMaterial.LightingModel

Shading that incorporates ambient and diffuse properties only.

static let phong: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Phong formula.

static let shadowOnly: SCNMaterial.LightingModel

