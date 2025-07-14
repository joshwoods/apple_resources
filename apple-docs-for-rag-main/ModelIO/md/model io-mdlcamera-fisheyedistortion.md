

- Model I/O
- MDLCamera
-  fisheyeDistortion 

Instance Property

# fisheyeDistortion

The second coefficient for determining the radial distortion applied to pixels rendered using the camera.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var fisheyeDistortion: Float { get set }
```

## Discussion

Light passing through any lens produces some amount of radial distortion, which a renderer can compute based on the focalLength property. However, some lenses or aesthetic designs introduce additional distortion. A renderer can model radial distortion using the following equation, in which `r` is the radial distance from a pixel to be rendered to the center of the projection, and `r’` is the new radial distance to that pixel accounting for distortion:

`r' = r * (1 +` barrelDistortion `* r^2 +` fisheyeDistortion `* r^4)`

A nonzero barrelDistortion value sufficiently describes the distortion characteristic of most lenses. To simulate other lenses—such as security cameras, plastic toy lenses, or VR headsets—use both the barrelDistortion and fisheyeDistortion properties. The default value of both radial distortion parameters is zero, resulting in a rectilinear projection.

## See Also

### Modeling a Physical Lens

var barrelDistortion: Float

The first coefficient for determining the radial distortion applied to pixels rendered using the camera.

var opticalVignetting: Float

The amount of radial light attenuation around the edges of an image rendered using the camera.

var chromaticAberration: Float

The amount of radial color shift around the edges of an image rendered using the camera.

var focalLength: Float

The focal length, in millimeters, of the camera’s simulated lens.

var fStop: Float

The relative aperture ratio of the camera’s simulated lens.

var apertureBladeCount: Int

The number of blades in the camera’s simulated aperture.

func bokehKernel(withSize: vector_int2) -> MDLTexture

Creates and returns a texture, based on the camera’s aperture blade count, to be used in rendering out-of-focus highlights in a scene.

var maximumCircleOfConfusion: Float

The maximum diameter, in millimeters on the imaging plane, at which light from a point source should appear in an image rendered using the camera.

var focusDistance: Float

The distance, in meters, at which the lens is focused.

var shutterOpenInterval: TimeInterval

The duration, in seconds, for which the camera’s simulated shutter is open during each frame.

