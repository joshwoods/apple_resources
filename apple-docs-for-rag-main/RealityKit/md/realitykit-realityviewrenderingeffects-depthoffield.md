

- RealityKit
- RealityViewRenderingEffects
-  depthOfField 

Instance Property

# depthOfField

Enables or disables a depth of field effect for virtual content.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var depthOfField: RealityViewRenderingEffectMode
```

## Discussion

When you set the focal point of a camera, you actually choose a range of focus rather than a point. Objects outside the range — either too close or too far away — appear out of focus, while objects inside the range appear in focus. The size of the range, known as the depth of field, depends on characteristics of the lens, the focal point, and other factors.

If you place a virtual object outside of the range of focus, it can appear detached from the scene in which it appears unless you blur the object to match its surroundings. In many cases, the depth of field is large enough that this doesn’t matter. But if it does matter for your app, you can enable a post-processing effect that blurs virtual objects to account for depth of field.

| Without depth of field | With depth of field |
|----|----|
|  |  |

Because of its computational cost, RealityView does not apply depth of field by default. To enable depth of field, set the `depthOfField` property of the view’s renderingEffects. If you do enable depth of field, be sure to check your app’s performance, as described in Improving the Performance of a RealityKit App.

Important

This rendering effect is unavailable on macOS.

