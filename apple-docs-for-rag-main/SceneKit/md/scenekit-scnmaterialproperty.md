

- SceneKit
-  SCNMaterialProperty 

Class

# SCNMaterialProperty

A container for the color or texture of one of a material’s visual properties.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNMaterialProperty
```

## Overview

A material has several visual properties that together determine its appearance under lighting and shading. SceneKit renders each pixel in the scene by combining the information from material properties with the locations, intensities, and colors of lights.

A material property’s contents can be either a color, which provides a uniform effect across the surface of a material, or a texture, which SceneKit maps across the surface of a material using texture coordinates provided by the geometry object the material is attached to. A texture, in turn, can come from any of several sources, such as an image object, a URL to an image file, a specially formatted image or set of images for use as a cube map, or even animated content provided by Core Animation, SpriteKit, or AVFoundation—for the full set of options, see the contents property.

Note

Typically, you associate texture images with materials when creating 3D assets with third-party authoring tools, and the scene files containing those assets reference external image files. For best results when shipping assets in your app bundle, place scene files in a folder with the `.scnassets` extension, and place image files referenced as textures from those scenes in an Asset Catalog.

Xcode then optimizes the scene and texture resources for best performance on each target device, and prepares your texture resources for delivery features such as App Thinning and On-Demand Resources.

SceneKit uses the material property’s contents object in different ways for each visual property of a material. For example:

- When you provide a color for the diffuse property, it determines the material’s base color—geometries using the material appear shaded in gradations of this color when illuminated by white light. If you instead provide an image, SceneKit maps the image across the geometry’s surface instead of shading with a uniform base color.

- When you provide a color for the specular property, it affects the color of light reflected directly toward the viewer from the surface of a geometry using the material. If you instead provide a grayscale image, it determines the tendency of the material to reflect light directly toward the viewer—lighter pixels in the image make those areas of the material appear more shiny, and darker pixels make the material appear more matte.

- The normal property specifies the orientation of a surface at each point. Materials are uniformly smooth by default, so specifying a color for this property has no useful effect. Instead, you can specify an image for this property that describes the contours of the surface. SceneKit uses this image (called a normal map) in lighting, creating the illusion of a complex, bumpy surface without increasing the complexity of the geometry.

For more details on each visual property and the ways their contents affect a material’s appearance, see SCNMaterial.

SceneKit also uses SCNMaterialProperty objects elsewhere:

- To provide content to be rendered behind a scene, in the background property of an SCNScene object,

- To affect the color and shape of illumination from a light source, in the gobo property of an SCNLight object.

- To bind texture samplers to custom GLSL shader source code snippets, in classes conforming to the SCNShadable protocol.

## Topics

### Creating a Material Property

convenience init(contents: Any)

Creates a new material property object with the specified contents.

### Working with Material Property Contents

var contents: Any?

The visual contents of the material property—a color, image, or source of animated content. Animatable.

var intensity: CGFloat

A number between `0.0` and `1.0` that modulates the effect of the material property. Animatable.

### Configuring Texture Mapping Attributes

var contentsTransform: SCNMatrix4

The transformation applied to the material property’s visual contents. Animatable.

var wrapS: SCNWrapMode

The wrapping behavior for the S texture coordinate.

var wrapT: SCNWrapMode

The wrapping behavior for the T texture coordinate.

enum SCNWrapMode

Modes to apply to texture wrapping, used by the wrapT and wrapS properties.

var minificationFilter: SCNFilterMode

Texture filtering for rendering the material property’s image contents at a size smaller than that of the original image.

var magnificationFilter: SCNFilterMode

Texture filtering for rendering the material property’s image contents at a size larger than that of the original image.

var mipFilter: SCNFilterMode

Texture filtering for using mipmaps to render the material property’s image contents at a size smaller than that of the original image.

enum SCNFilterMode

Texture filtering modes, used by the minificationFilter, magnificationFilter, and mipFilter properties.

var maxAnisotropy: CGFloat

The amount of anisotropic texture filtering to be used when rendering the material property’s image contents.

var mappingChannel: Int

The source of texture coordinates for mapping the material property’s image contents.

var borderColor: Any?

A color used to fill in areas of a material’s surface not covered by the material property’s image contents.

Deprecated

### Instance Properties

var textureComponents: SCNColorMask

### Type Methods

class func precomputedLightingEnvironmentContents(with: Data) throws -> Any

class func precomputedLightingEnvironmentContents(with: URL) throws -> Any

class func precomputedLightingEnvironmentData(forContents: Any, device: (any MTLDevice)?) throws -> Data

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
- NSObjectProtocol
- NSSecureCoding
- SCNAnimatable

## See Also

### Lighting, Cameras, and Shading

class SCNLight

A light source that can be attached to a node to illuminate the scene.

class SCNCamera

A set of camera attributes that can be attached to a node to provide a point of view for displaying the scene.

class SCNMaterial

A set of shading attributes that define the appearance of a geometry’s surface when rendered.

