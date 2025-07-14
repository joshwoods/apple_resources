

- RealityKit
- ARView
- ARView.RenderOptions
-  disablePersonOcclusion 

Type Property

# disablePersonOcclusion

Disable person segmentation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
static let disablePersonOcclusion: ARView.RenderOptions
```

## Discussion

By default, ARKit detects users in the frame, and hides content occluded by users. Add the disablePersonOcclusion option to the AR view’s renderOptions to disable this feature.

## See Also

### Disabling rendering effects

static let disableCameraGrain: ARView.RenderOptions

Disable the image noise effect.

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

static let disableAREnvironmentLighting: ARView.RenderOptions

Disable lighting from environment probes.

static let disableFaceOcclusions: ARView.RenderOptions

Disable automatic face occlusion.

Deprecated

static let disableAutomaticLighting: ARView.RenderOptions

Disable automatic updates of the scene lighting.

Deprecated

