

- RealityKit
- ARView
- ARView.RenderOptions
-  disableGroundingShadows 

Type Property

# disableGroundingShadows

Disable rendering of ambient occlusion and shadows that ground objects in an AR scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
static let disableGroundingShadows: ARView.RenderOptions
```

## Discussion

Objects in the real world cast a grounding shadow onto adjacent surfaces due to ambient light. This provides viewers with a visual cue that the object is in close proximity to the surface. Objects without a grounding shadow appear disconnected from their environment. To create the same visual cue for virtual objects, RealityKit provides a grounding shadow effect.

Applying this effect involves a low, constant GPU cost. You can disable the effect by adding the disableGroundingShadows option to the view’s renderOptions set, if needed. Disabling the effect is most useful for older devices, like those with an A9 processor or earlier.

## See Also

### Disabling rendering effects

static let disableCameraGrain: ARView.RenderOptions

Disable the image noise effect.

static let disableHDR: ARView.RenderOptions

Disable the high dynamic range post-processing effect.

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

