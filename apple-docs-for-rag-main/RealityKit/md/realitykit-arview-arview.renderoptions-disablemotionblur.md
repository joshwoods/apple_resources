

- RealityKit
- ARView
- ARView.RenderOptions
-  disableMotionBlur 

Type Property

# disableMotionBlur

Disable the motion blur for all virtual content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
static let disableMotionBlur: ARView.RenderOptions
```

## Mentioned in 

Reducing GPU Utilization in Your RealityKit App

## Discussion

A video stream consists of a sequence of images. Each image in the sequence represents a short, but non-zero period of time. Fast-moving, real-world objects captured within a frame can experience a visual smearing, known as *motion blur*.

By default, virtual objects that appear in the scene don’t experience motion blur. Instead, they exist at exactly one point in the frame for any given image in the image sequence. RealityKit offers an effect that introduces motion blur for virtual objects, taking into account the relative motion of the camera and the object.

Because of its computational cost, motion blur is off by default on all but the latest hardware. To enable or disable the effect, you add or remove the disableMotionBlur option to or from the renderOptions set, respectively. If you do enable motion blur, be sure to measure your app’s CPU and GPU utilization to find out how it affects your app’s performance, as described in Improving the Performance of a RealityKit App.

## See Also

### Disabling rendering effects

static let disableCameraGrain: ARView.RenderOptions

Disable the image noise effect.

static let disableHDR: ARView.RenderOptions

Disable the high dynamic range post-processing effect.

static let disableGroundingShadows: ARView.RenderOptions

Disable rendering of ambient occlusion and shadows that ground objects in an AR scene.

static let disableDepthOfField: ARView.RenderOptions

Disable the depth of field effect for all virtual content.

static let disableFaceMesh: ARView.RenderOptions

Disable generation of the face entity with the default occlusion material.

static let disablePersonOcclusion: ARView.RenderOptions

Disable person segmentation.

static let disableAREnvironmentLighting: ARView.RenderOptions

Disable lighting from environment probes.

static let disableFaceOcclusions: ARView.RenderOptions

Disable automatic face occlusion.

Deprecated

static let disableAutomaticLighting: ARView.RenderOptions

Disable automatic updates of the scene lighting.

Deprecated

