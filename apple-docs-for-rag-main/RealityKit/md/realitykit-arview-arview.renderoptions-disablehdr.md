

- RealityKit
- ARView
- ARView.RenderOptions
-  disableHDR 

Type Property

# disableHDR

Disable the high dynamic range post-processing effect.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
static let disableHDR: ARView.RenderOptions
```

## Discussion

RealityKit applies a high dynamic range effect, along with tone mapping, as a post-processing step in the GPU during the render. This effect is computationally inexpensive, but you can add the disableHDR option to the view’s renderOptions set to turn the effect off, if needed. Disabling the effect is most useful on older devices, like those with an A9 processor or earlier.

When deciding whether to use any effect, be sure to consider your app’s CPU and GPU utilization, as described in Improving the Performance of a RealityKit App.

## See Also

### Disabling rendering effects

static let disableCameraGrain: ARView.RenderOptions

Disable the image noise effect.

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

