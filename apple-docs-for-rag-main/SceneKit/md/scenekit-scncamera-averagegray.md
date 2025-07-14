

- SceneKit
- SCNCamera
-  averageGray 

Instance Property

# averageGray

The luminance level to use as the midpoint of a tone mapping curve.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var averageGray: CGFloat { get set }
```

## Discussion

When using a High Dynamic Range (HDR) camera, SceneKit applies a process called *tone mapping* to translate the wide range of luminance values in the visible scene to the narrower range of brightness values that can be shown on a display. SceneKit determines a tone mapping curve from the minimumExposure, maximumExposure, exposureOffset, and whitePoint properties, along with this property which serves as a constant estimate of scene luminance.

The default value is `0.18`. By setting this property to a higher or lower value, you can compensate for scenes with darker or brighter content. Alternatively, by setting the wantsExposureAdaptation property, you can allow SceneKit to automatically adjust exposure as the visible contents of the scene change.

This property has no effect if the wantsHDR value is false. If the exposureAdaptationDarkeningSpeedFactor value is true, SceneKit ignores this property, and instead computes the average luminance currently visible to the camera during rendering.

## See Also

### Adding High Dynamic Range Effects

var wantsHDR: Bool

A Boolean value that determines whether SceneKit applies High Dynamic Range (HDR) postprocessing effects to a scene.

var exposureOffset: CGFloat

A logarithmic bias that adjusts the results of SceneKit’s tone mapping operation, brightening or darkening the visible scene.

var whitePoint: CGFloat

The luminance level to use as the upper end of a tone mapping curve.

var minimumExposure: CGFloat

The minimum exposure value to use in tone mapping.

var maximumExposure: CGFloat

The minimum exposure value to use in tone mapping.

