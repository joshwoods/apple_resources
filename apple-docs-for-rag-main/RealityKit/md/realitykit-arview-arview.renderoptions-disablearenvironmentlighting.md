

- RealityKit
- ARView
- ARView.RenderOptions
-  disableAREnvironmentLighting 

Type Property

# disableAREnvironmentLighting

Disable lighting from environment probes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
static let disableAREnvironmentLighting: ARView.RenderOptions
```

## Discussion

By default, RealityKit automatically creates light probes to record the lighting conditions both globally, and at appropriate points in the scene. The framework adjusts the complexity of the light probe set to match the capabilities of the GPU. For example, it might use only a global probe on less capable devices. It then applies environment lighting to virtual objects based on the probes.

To disable this effect, add this option to the renderOptions set.

Alternatively, to use environment lighting but control the probes manually, ensure the render option set doesn’t include this option. Then configure the session for manual environment texturing, using the ARWorldTrackingConfiguration.EnvironmentTexturing.manual value.

For more information about creating and placing probes manually, see Adding realistic reflections to an AR experience.

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

static let disablePersonOcclusion: ARView.RenderOptions

Disable person segmentation.

static let disableFaceOcclusions: ARView.RenderOptions

Disable automatic face occlusion.

Deprecated

static let disableAutomaticLighting: ARView.RenderOptions

Disable automatic updates of the scene lighting.

Deprecated

