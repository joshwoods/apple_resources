

- SceneKit
- SCNCamera
-  exposureAdaptationDarkeningSpeedFactor 

Instance Property

# exposureAdaptationDarkeningSpeedFactor

The relative duration of automatically animated exposure transitions from bright to dark areas.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var exposureAdaptationDarkeningSpeedFactor: CGFloat { get set }
```

## Discussion

When using a High Dynamic Range (HDR) camera, SceneKit applies a process called *tone mapping* to translate the wide range of luminance values in the visible scene to the narrower range of brightness values that can be shown on a display. When the wantsExposureAdaptation property is enabled, SceneKit automatically adjusts the tone mapping curve based on the average luminance currently visible to the camera, and creates automatic transitions between exposure levels.

SceneKit automatically determines the overall duration of exposure-level animations based on the values of this property and the exposureAdaptationDarkeningSpeedFactor property. The default value is `0.6`, resulting in darkening animations that are slightly faster than brighting animations.

This property has no effect if either of the wantsHDR or wantsExposureAdaptation values is false.

## See Also

### Adding Automatic HDR Exposure Adaptation

var wantsExposureAdaptation: Bool

A Boolean value that determines whether SceneKit automatically adjusts the exposure level.

var exposureAdaptationBrighteningSpeedFactor: CGFloat

The relative duration of automatically animated exposure transitions from dark to bright areas.

