

- ARKit
- ARDirectionalLightEstimate
-  primaryLightDirection 

Instance Property

# primaryLightDirection

A vector indicating the orientation of the strongest directional light source in the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var primaryLightDirection: simd_float3 { get }
```

## Discussion

When ARKit analyzes the directional lighting environment for a detected face, the resulting lighting estimate can represent the influence of multiple light sources with different directions and intensities. To access this level of detail for use in your custom rendering code, use the sphericalHarmonicsCoefficients property.

If your app displays AR content using a technology that doesn’t support environment-based lighting, this primaryLightDirection property represents the average of directional light sources in the scene. This vector is normalized and in world coordinate space.

## See Also

### Examining Light Parameters

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions.

var primaryLightIntensity: CGFloat

The estimated intensity, in lumens, of the strongest directional light source in the scene.

