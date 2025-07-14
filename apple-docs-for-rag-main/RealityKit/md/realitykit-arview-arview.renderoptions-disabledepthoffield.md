

- RealityKit
- ARView
- ARView.RenderOptions
-  disableDepthOfField 

Type Property

# disableDepthOfField

Disable the depth of field effect for all virtual content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
static let disableDepthOfField: ARView.RenderOptions
```

## Discussion

When you set the focal point of a camera, you actually choose a range of focus rather than a point. Objects outside the range — either too close or too far away — appear out of focus, while objects inside the range appear in focus. The size of the range, known as the depth of field, depends on characteristics of the lens, the focal point, and other factors.

If you place a virtual object outside of the range of focus, it can appear detached from the scene in which it appears unless you blur the object to match its surroundings. In many cases, the depth of field is large enough that this doesn’t matter. But if it does matter for your app, you can enable a post-processing effect that blurs virtual objects to account for depth of field.

| Without depth of field | With depth of field |
|----|----|
|  |  |

Because of its computational cost, the system disables depth of field by default when you create a new ARView instance. To enable depth of field, remove the disableDepthOfField option from the renderOptions set. If you do enable depth of field, be sure to check your app’s performance, as described in Improving the Performance of a RealityKit App.

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

