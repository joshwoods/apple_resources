

- SceneKit
-  SCNLight 

Class

# SCNLight

A light source that can be attached to a node to illuminate the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNLight
```

## Overview

You illuminate your scene by attaching lights to SCNNode objects using their light property.

You set a light’s type using its type property. Depending on a light’s type, its position and direction may affect its behavior—you control the light’s position and direction through the node that the light is attached to. The direction of a light, if applicable to its type, is along the negative z-axis of its node’s local coordinate system.

A light’s other properties affect how it illuminates a scene. All lights have a color property, which interacts with SCNMaterial objects to produce the pixel colors in a rendered scene. Other properties, such as attenuation, shadowing, and spot angle, can affect the behavior of certain types of lights.

The number and type of lights in a scene is a key factor in SceneKit’s rendering performance. For efficient rendering, follow these tips:

- Use SceneKit lights only for dynamic light sources or lights that affect moving objects. For statically lit portions of your scene, create a light map texture in an external 3D authoring tool (also known as *baked lighting*) and apply it to objects in the scene using the multiply material property.

- Minimize the number of lights on each element of the scene. You can achieve most common lighting effects using no more than three lights, and you only need a single ambient light source. SceneKit only uses up to eight light sources per node when rendering, ignoring any additional lights. If you set the attenuationEndDistance property on a spotlight or omnidirectional light to limit its area of effect, SceneKit ignores the light (and its performance cost) when rendering objects outside that area. You can also use the categoryBitMask property to choose which nodes are illuminated by a light.

## Topics

### Modifying a Light’s Appearance

var type: SCNLight.LightType

A constant identifying the general behavior of the light.

struct LightType

Constants specifying the general behavior of a light, used by the type property.

var color: Any

The color of the light. Animatable.

var temperature: CGFloat

The color temperature, in degrees Kelvin, of the light source. Animatable.

var intensity: CGFloat

The luminous flux, in lumens, or total brightness of the light. Animatable.

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions for a light probe.

### Managing Light Attributes

var name: String?

A name associated with the light.

func attribute(forKey: String) -> Any?

Returns the value of a lighting attribute.

Deprecated

func setAttribute(Any?, forKey: String)

Sets the value for a lighting attribute.

Deprecated

Lighting Attribute Keys

Keys for specifying the behavior of a light using the attribute(forKey:) and setAttribute(_:forKey:) methods.

### Managing Light Attenuation

var attenuationStartDistance: CGFloat

The distance from the light at which its intensity begins to diminish. Animatable.

var attenuationEndDistance: CGFloat

The distance from the light at which its intensity is completely diminished. Animatable.

var attenuationFalloffExponent: CGFloat

The transition curve for the light’s intensity between its attenuation start and end distances. Animatable.

### Managing Spotlight Extent

var spotInnerAngle: CGFloat

The angle, in degrees, of the area fully lit by a spotlight. Animatable.

var spotOuterAngle: CGFloat

The angle, in degrees, of the area partially lit by a spotlight. Animatable.

var gobo: SCNMaterialProperty?

An image or other visual content affecting the shape and color of a light’s illuminated area.

### Managing Shadows Cast by the Light

var castsShadow: Bool

A Boolean value that determines whether the light casts shadows.

var shadowRadius: CGFloat

A number that specifies the amount of blurring around the edges of shadows cast by the light. Animatable.

var shadowColor: Any

The color of shadows cast by the light. Animatable.

var shadowMapSize: CGSize

The size of the shadow map image that SceneKit renders when creating shadows.

var shadowSampleCount: Int

The number of samples from the shadow map that SceneKit uses to render each pixel.

var shadowMode: SCNShadowMode

The mode SceneKit uses to render shadows.

enum SCNShadowMode

Options for SceneKit’s rendering of shadows cast by a light, used by the shadowMode property.

var shadowBias: CGFloat

The amount of correction to apply to the shadow to prevent rendering artifacts.

var orthographicScale: CGFloat

The orthographic scale SceneKit uses when rendering the shadow map for a directional light.

var zFar: CGFloat

The maximum distance between the light and a visible surface for casting shadows.

var zNear: CGFloat

The minimum distance between the light and a visible surface for casting shadows. Animatable.

### Choosing Nodes to be Illuminated by the Light

var categoryBitMask: Int

A mask that defines which categories this light belongs to.

### Managing Photometric Lights

var iesProfileURL: URL?

The URL for a file that contains photometry data describing the intended appearance of the light.

### Instance Properties

var areaExtents: simd_float3

var areaPolygonVertices: [NSValue]?

var areaType: SCNLightAreaType

var automaticallyAdjustsShadowProjection: Bool

var doubleSided: Bool

var drawsArea: Bool

var forcesBackFaceCasters: Bool

var maximumShadowDistance: CGFloat

var parallaxCenterOffset: simd_float3

var parallaxCorrectionEnabled: Bool

var parallaxExtentsFactor: simd_float3

var probeEnvironment: SCNMaterialProperty?

var probeExtents: simd_float3

var probeOffset: simd_float3

var probeType: SCNLightProbeType

var probeUpdateType: SCNLightProbeUpdateType

var sampleDistributedShadowMaps: Bool

var shadowCascadeCount: Int

var shadowCascadeSplittingFactor: CGFloat

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- SCNAnimatable
- SCNTechniqueSupport

## See Also

### Lighting, Cameras, and Shading

class SCNCamera

A set of camera attributes that can be attached to a node to provide a point of view for displaying the scene.

class SCNMaterial

A set of shading attributes that define the appearance of a geometry’s surface when rendered.

class SCNMaterialProperty

A container for the color or texture of one of a material’s visual properties.

