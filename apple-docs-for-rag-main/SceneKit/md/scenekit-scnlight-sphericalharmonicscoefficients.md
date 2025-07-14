

- SceneKit
- SCNLight
-  sphericalHarmonicsCoefficients 

Instance Property

# sphericalHarmonicsCoefficients

Data describing the estimated lighting environment in all directions for a light probe.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var sphericalHarmonicsCoefficients: Data { get }
```

## Discussion

Spherical harmonic coefficients describe the distribution of light around a point in a format that can be used efficiently in real-time rendering. SceneKit supports spherical harmonics only for lights of the probe type.

The data is an 32-bit floating-point values, containing three noninterleaved data sets corresponding to the red, green, and blue sets of coefficients. SceneKit supports only level 2 spherical harmonics, so the array has 3 sets of 9 values, or 27 values total.

## See Also

### Related Documentation

class ARDirectionalLightEstimate

Estimated environmental lighting information associated with a captured video frame in a face-tracking AR session.

class MDLLightProbe

A light source described in terms of the variations in color and intensity of its illumination in all directions.

### Modifying a Light’s Appearance

var type: SCNLight.LightType

A constant identifying the general behavior of the light.

struct LightType

Constants specifying the general behavior of a light, used by the type property.

var color: Any

The color of the light. Animatable.

var temperature: CGFloat

The color temperature, in degrees Kelvin, of the light source. Animatable.

var intensity: CGFloat

The luminous flux, in lumens, or total brightness of the light. Animatable.

