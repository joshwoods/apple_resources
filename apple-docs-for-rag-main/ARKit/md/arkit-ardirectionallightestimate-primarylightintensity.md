

- ARKit
- ARDirectionalLightEstimate
-  primaryLightIntensity 

Instance Property

# primaryLightIntensity

The estimated intensity, in lumens, of the strongest directional light source in the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var primaryLightIntensity: CGFloat { get }
```

## Discussion

When ARKit analyzes the directional lighting environment for a detected face, the resulting lighting estimate can represent the influence of multiple light sources with different directions and intensities. To access this level of detail for use in your custom rendering code, use the sphericalHarmonicsCoefficients property.

If your app displays AR content using a technology that doesn’t support environment-based lighting, this primaryLightIntensity property represents the average of directional light sources in the scene. This value is scaled to be appropriate for use in rendering architectures that use realistic lighting metrics, with a value of 1000 representing neutral lighting.

For example, you can pass this value directly to the intensity property of a SceneKit directional light for lighting results that roughly match those of the real-world scene captured by the device camera. (However, passing this value to SceneKit is generally not necessary; the ARSCNView class automatically sets SceneKit lighting based on the sphericalHarmonicsCoefficients property.)

## See Also

### Examining Light Parameters

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions.

var primaryLightDirection: simd_float3

A vector indicating the orientation of the strongest directional light source in the scene.

