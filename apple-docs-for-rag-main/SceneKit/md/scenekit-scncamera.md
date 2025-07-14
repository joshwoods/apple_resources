

- SceneKit
-  SCNCamera 

Class

# SCNCamera

A set of camera attributes that can be attached to a node to provide a point of view for displaying the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SCNCamera
```

## Overview

To display a scene, you must designate a node whose camera property contains a camera object as the point of view.

The SCNNode object containing a camera defines a point of view—that is, the position and orientation of the camera. A camera’s direction of view is always along the negative z-axis of the node’s local coordinate system. To point the camera at different parts of your scene, use the position, rotation, or transform property of the node containing it. (Alternatively, to ensure that a camera always points at a particular element of your scene even when that element moves, attach a SCNLookAtConstraint object to the node containing the camera.)

An SCNCamera object itself defines the shape and, in part, the appearance of the rendered scene as seen from its point of view. By default, a camera defines a perspective projection, whose field of view (FOV) and near and far visibility limits you control using the properties listed in Adjusting Camera Perspective and illustrated below.

## Topics

### Managing Camera Attributes

var name: String?

A name associated with the camera object.

### Adjusting Camera Perspective

var zNear: Double

The camera’s near depth limit. Animatable.

var zFar: Double

The camera’s far depth limit. Animatable.

var automaticallyAdjustsZRange: Bool

A Boolean value that determines whether the camera automatically adjusts its zNear and zFar depth limits.

### Managing Field of View

var fieldOfView: CGFloat

The vertical or horizontal viewing angle of the camera.

var focalLength: CGFloat

The camera’s focal length, in millimeters.

var sensorHeight: CGFloat

The vertical size of the camera’s imaging plane, in millimeters.

var projectionDirection: SCNCameraProjectionDirection

The axis used to determine field of view or orthographic scale.

enum SCNCameraProjectionDirection

Options for the axis used to determine field of view or orthographic projection.

### Managing the Projection Transform

var projectionTransform: SCNMatrix4

The camera’s projection transformation.

var usesOrthographicProjection: Bool

A Boolean value that determines whether the camera uses an orthographic projection.

var orthographicScale: Double

Specifies the camera’s magnification factor when using an orthographic projection.

### Choosing Nodes to Be Visible to the Camera

var categoryBitMask: Int

A mask that defines which categories this camera belongs to.

### Adding Depth-of-Field Effects

var wantsDepthOfField: Bool

A Boolean value that determines whether SceneKit renders depth-of-field blur effects for the camera.

var focusDistance: CGFloat

The distance from the camera at which objects appear in sharp focus. Animatable.

var fStop: CGFloat

The physical camera aperture simulated by SceneKit for depth-of-field effects. Animatable.

var apertureBladeCount: Int

The number of physical camera aperture blades simulated by SceneKit for depth-of-field effects.

var focalBlurSampleCount: Int

The number of pixel samples SceneKit uses to create depth-of-field blur effects.

### Adding Motion Blur Effects

var motionBlurIntensity: CGFloat

A factor that determines the intensity of motion blur effects. Animatable.

### Adding High Dynamic Range Effects

var wantsHDR: Bool

A Boolean value that determines whether SceneKit applies High Dynamic Range (HDR) postprocessing effects to a scene.

var exposureOffset: CGFloat

A logarithmic bias that adjusts the results of SceneKit’s tone mapping operation, brightening or darkening the visible scene.

var averageGray: CGFloat

The luminance level to use as the midpoint of a tone mapping curve.

var whitePoint: CGFloat

The luminance level to use as the upper end of a tone mapping curve.

var minimumExposure: CGFloat

The minimum exposure value to use in tone mapping.

var maximumExposure: CGFloat

The minimum exposure value to use in tone mapping.

### Adding Automatic HDR Exposure Adaptation

var wantsExposureAdaptation: Bool

A Boolean value that determines whether SceneKit automatically adjusts the exposure level.

var exposureAdaptationBrighteningSpeedFactor: CGFloat

The relative duration of automatically animated exposure transitions from dark to bright areas.

var exposureAdaptationDarkeningSpeedFactor: CGFloat

The relative duration of automatically animated exposure transitions from bright to dark areas.

### Adjusting Rendered Colors

var contrast: CGFloat

An adjustment factor to apply to the overall visual contrast of the rendered scene.

var saturation: CGFloat

An adjustment factor to apply to the overall color saturation of the rendered scene.

var colorGrading: SCNMaterialProperty

A texture for applying color grading effects to the entire rendered scene.

### Adding Stylistic Visual Effects

var bloomIntensity: CGFloat

The magnitude of bloom effect to apply to highlights in the rendered scene. Animatable.

var bloomThreshold: CGFloat

The brightness threshold at which to apply a bloom effect to highlights in the rendered scene. Animatable.

var bloomBlurRadius: CGFloat

The radius, in pixels, for the blurring portion of the bloom effect applied to highlights in the rendered scene. Animatable.

var colorFringeIntensity: CGFloat

The blend factor for fading the color fringing effect applied to the rendered scene.

var colorFringeStrength: CGFloat

The magnitude of color fringing effect to apply to the rendered scene.

var vignettingIntensity: CGFloat

The magnitude of vignette (darkening around edges) effect to apply to the rendered scene.

var vignettingPower: CGFloat

The amount of the rendered scene to darken with a vignette effect.

### Adding Screen-Space Ambient Occlusion

var screenSpaceAmbientOcclusionIntensity: CGFloat

The intensity of the screen-space ambient occlusion effect applied in camera rendering.

var screenSpaceAmbientOcclusionRadius: CGFloat

The distance, in units of scene space, at which ambient occlusion takes effect.

var screenSpaceAmbientOcclusionBias: CGFloat

An offset for modulating ambient occlusion effects.

var screenSpaceAmbientOcclusionDepthThreshold: CGFloat

The maximum depth difference, in units of scene space, at which to apply ambient occlusion effects.

var screenSpaceAmbientOcclusionNormalThreshold: CGFloat

The magnitude of the blur effect applied to create ambient occlusion shadows.

### Deprecated

var yFov: Double

The camera’s field of view, in degrees, on the vertical axis. Animatable.

Deprecated

var xFov: Double

The camera’s field of view, in degrees, on the horizontal axis. Animatable.

Deprecated

var focalDistance: CGFloat

The distance from the camera at which objects appear in sharp focus. Animatable.

Deprecated

var focalSize: CGFloat

The width of the distance range at which objects appear in sharp focus. Animatable.

Deprecated

var focalBlurRadius: CGFloat

The maximum amount of blurring, in pixels, applied to areas outside the camera’s depth of field. Animatable.

Deprecated

var aperture: CGFloat

A factor that determines the transition between in-focus and out-of-focus areas. Animatable.

Deprecated

### Instance Properties

var bloomIterationCount: Int

var bloomIterationSpread: CGFloat

var grainIntensity: CGFloat

var grainIsColored: Bool

var grainScale: CGFloat

var whiteBalanceTemperature: CGFloat

var whiteBalanceTint: CGFloat

### Instance Methods

func projectionTransform(withViewportSize: CGSize) -> SCNMatrix4

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
- SCNTechniqueSupport

## See Also

### Lighting, Cameras, and Shading

class SCNLight

A light source that can be attached to a node to illuminate the scene.

class SCNMaterial

A set of shading attributes that define the appearance of a geometry’s surface when rendered.

class SCNMaterialProperty

A container for the color or texture of one of a material’s visual properties.

