

- Model I/O
- MDLCamera
-  focusDistance 

Instance Property

# focusDistance

The distance, in meters, at which the lens is focused.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var focusDistance: Float { get set }
```

## Discussion

A renderer can produce out-of-focus blur effects for objects significantly nearer to or farther from the camera than this distance. The default is 2.5 meters.

## See Also

### Modeling a Physical Lens

var barrelDistortion: Float

The first coefficient for determining the radial distortion applied to pixels rendered using the camera.

var fisheyeDistortion: Float

The second coefficient for determining the radial distortion applied to pixels rendered using the camera.

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

var shutterOpenInterval: TimeInterval

The duration, in seconds, for which the camera’s simulated shutter is open during each frame.

