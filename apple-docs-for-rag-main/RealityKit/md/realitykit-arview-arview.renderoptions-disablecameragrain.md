

- RealityKit
- ARView
- ARView.RenderOptions
-  disableCameraGrain 

Type Property

# disableCameraGrain

Disable the image noise effect.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
static let disableCameraGrain: ARView.RenderOptions
```

## Discussion

Images from a camera may contain a small amount of noise, called *camera grain*, that increases as the available light decreases. Virtual objects rendered without noise and placed into an otherwise grainy image look out of place. You can use RealityKit to add noise to the rendered output to match noise in the camera feed.

| Without camera grain | With camera grain |
|----|----|
|  |  |

Applying this effect involves a low, constant GPU cost. If necessary, you can disable the effect by adding the disableCameraGrain option to the view’s renderOptions set. Disabling the effect is most useful for older devices, like those with an A9 processor or earlier.

When deciding whether to use any effect, be sure to consider your app’s CPU and GPU utilization, as described in Improving the Performance of a RealityKit App.

## See Also

### Disabling rendering effects

static let disableHDR: ARView.RenderOptions

Disable the high dynamic range post-processing effect.

static let disableGroundingShadows: ARView.RenderOptions

Disable rendering of ambient occlusion and shadows that ground objects in an AR scene.

static let disableMotionBlur: ARView.RenderOptions

Disable the motion blur for all virtual content.

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

