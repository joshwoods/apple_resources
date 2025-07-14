

- Model I/O
- MDLCamera
-  apertureBladeCount 

Instance Property

# apertureBladeCount

The number of blades in the camera’s simulated aperture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var apertureBladeCount: Int { get set }
```

## Discussion

The shape of a real-world camera’s aperture is determined by the number of overlapping blades that form an adjustable iris, whose center opening light passes through between the lens and the imaging surface (film or sensor). This shape affects that of out-of-focus highlights, commonly called *bokeh*, that appear in images seen by the camera. The aesthetic quality of a lens’ bokeh is one of the characteristics that drives the choice of a lens for a particular scene. To create a texture image for use in rendering bokeh highlights, use the bokehKernel(withSize:) method.

The default aperture blade count is zero, indicating a perfectly circular aperture.

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

func bokehKernel(withSize: vector_int2) -> MDLTexture

Creates and returns a texture, based on the camera’s aperture blade count, to be used in rendering out-of-focus highlights in a scene.

var maximumCircleOfConfusion: Float

The maximum diameter, in millimeters on the imaging plane, at which light from a point source should appear in an image rendered using the camera.

var focusDistance: Float

The distance, in meters, at which the lens is focused.

var shutterOpenInterval: TimeInterval

The duration, in seconds, for which the camera’s simulated shutter is open during each frame.

