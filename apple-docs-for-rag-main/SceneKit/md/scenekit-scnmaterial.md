

- SceneKit
-  SCNMaterial 

Class

# SCNMaterial

A set of shading attributes that define the appearance of a geometry’s surface when rendered.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNMaterial
```

## Overview

When you create a material, you define a collection of visual attributes and their options, which you can then reuse for multiple geometries in a scene.

A material has several visual properties, each of which defines a different part of SceneKit’s lighting and shading process. Each visual property is an instance of the SCNMaterialProperty class that provides a solid color, texture, or other 2D content for that aspect of SceneKit’s rendering. The material’s lightingModel property then determines the formula SceneKit uses to combine the visual properties with the lights in the scene to produce the final color for each pixel in the rendered scene. For more details on the rendering process, see SCNMaterial.LightingModel.

You attach one or more materials to an instance of the SCNGeometry class using its firstMaterial or materials property. Multiple geometries can reference the same material. In this case, changing the attributes of the material changes the appearance of every geometry that uses it.

## Topics

### Creating a Material

var name: String?

A name associated with the material.

### Choosing a Shading Model

var lightingModel: SCNMaterial.LightingModel

The lighting formula that SceneKit uses to render the material.

struct LightingModel

Constants specifying the lighting and shading algorithm to use for rendering a material.

### Visual Properties for Physically Based Shading

var diffuse: SCNMaterialProperty

An object that manages the material’s diffuse response to lighting.

var metalness: SCNMaterialProperty

An object that provides color values to determine how metallic the material’s surface appears.

var roughness: SCNMaterialProperty

An object that provides color values to determine the apparent smoothness of the surface.

### Visual Properties for Special Effects

var normal: SCNMaterialProperty

An object that defines the nominal orientation of the surface at each point for use in lighting.

var displacement: SCNMaterialProperty

var emission: SCNMaterialProperty

An object that defines the color emitted by each point on a surface.

var selfIllumination: SCNMaterialProperty

An object that provides color values representing the global illumination of the surface.

var ambientOcclusion: SCNMaterialProperty

An object that provides color values to be multiplied with the ambient light affecting the material.

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

var locksAmbientWithDiffuse: Bool

A Boolean value that determines whether the material responds identically to both ambient and diffuse lighting. Animatable.

### Managing Opacity and Blending

var transparency: CGFloat

The uniform transparency of the material. Animatable.

var transparencyMode: SCNTransparencyMode

The mode SceneKit uses to calculate transparency for the material.

enum SCNTransparencyMode

The modes SceneKit uses to calculate the opacity of pixels rendered with a material, used by the transparencyMode property.

var blendMode: SCNBlendMode

The mode that determines how pixel colors rendered using this material blend with other pixel colors in the rendering target.

enum SCNBlendMode

Modes that describe how SceneKit blends source colors rendered using a material with destination colors already in a rendering target, used by the blendMode property.

### Customizing Rendered Appearance

var isLitPerPixel: Bool

A Boolean value that determines whether SceneKit performs lighting calculations per vertex or per pixel. Animatable.

var isDoubleSided: Bool

A Boolean value that determines whether SceneKit renders both front and back faces of a surface.

var cullMode: SCNCullMode

The mode determining which faces of a surface SceneKit renders. Animatable.

enum SCNCullMode

The modes SceneKit uses to determine which polygons to render in a surface, used by the cullMode property.

var fillMode: SCNFillMode

enum SCNFillMode

### Managing Render Targets

var writesToDepthBuffer: Bool

A Boolean value that determines whether SceneKit produces depth information when rendering the material.

var readsFromDepthBuffer: Bool

A Boolean value that determines whether SceneKit uses depth information when rendering the material.

var colorBufferWriteMask: SCNColorMask

struct SCNColorMask

### Instance Properties

var clearCoat: SCNMaterialProperty

var clearCoatNormal: SCNMaterialProperty

var clearCoatRoughness: SCNMaterialProperty

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- SCNAnimatable
- SCNShadable

## See Also

### Lighting, Cameras, and Shading

class SCNLight

A light source that can be attached to a node to illuminate the scene.

class SCNCamera

A set of camera attributes that can be attached to a node to provide a point of view for displaying the scene.

class SCNMaterialProperty

A container for the color or texture of one of a material’s visual properties.

