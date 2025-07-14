

- RealityKit
- RealityViewRenderingEffects
-  dynamicRange 

Instance Property

# dynamicRange

Enables or disables high dynamic range rendering for virtual content.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var dynamicRange: RealityViewDynamicRange
```

## Discussion

RealityKit applies a high dynamic range effect, along with tone mapping, as a post-processing step in the GPU during the render. This effect is computationally inexpensive, but you can add the disableHDR option to the view’s renderOptions set to turn the effect off, if needed.

When deciding whether to use any effect, be sure to consider your app’s CPU and GPU utilization, as described in Improving the Performance of a RealityKit App.

Important

This rendering effect is unavailable on macOS.

