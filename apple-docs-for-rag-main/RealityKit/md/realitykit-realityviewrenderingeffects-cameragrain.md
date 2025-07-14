

- RealityKit
- RealityViewRenderingEffects
-  cameraGrain 

Instance Property

# cameraGrain

Enables or disables an image noise effect for virtual content.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var cameraGrain: RealityViewRenderingEffectMode
```

## Discussion

Images from a camera may contain a small amount of noise, called *camera grain*, that increases as the available light decreases. Virtual objects rendered without noise and placed into an otherwise grainy image look out of place. You can use RealityKit to add noise to the rendered output to match noise in the camera feed.

| Without camera grain | With camera grain |
|----|----|
|  |  |

Applying this effect involves a low, constant GPU cost. To enable or disable camera grain, set the `cameraGrain` property of the view’s renderingEffects.

When deciding whether to use any effect, be sure to consider your app’s CPU and GPU utilization, as described in Improving the Performance of a RealityKit App.

Important

This rendering effect is unavailable on macOS.

