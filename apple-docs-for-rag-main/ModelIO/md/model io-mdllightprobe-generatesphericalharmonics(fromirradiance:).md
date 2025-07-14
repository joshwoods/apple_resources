

- Model I/O
- MDLLightProbe
-  generateSphericalHarmonics(fromIrradiance:) 

Instance Method

# generateSphericalHarmonics(fromIrradiance:)

Generates spherical harmonics information based on the light probe’s irradiance texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func generateSphericalHarmonics(fromIrradiance sphericalHarmonicsLevel: Int)
```

## Parameters 

`sphericalHarmonicsLevel`  

The number of levels for which to generate spherical harmonics. Each level of spherical harmonics contains more coefficients, affecting both the layout of the resulting data and the detail of any lighting effects based on it.

## Discussion

Spherical harmonic coefficients describe the distribution of light around a light source with less high-frequency detail than a cube map texture, but they can be used more efficiently in real-time rendering. After calling this method, use the sphericalHarmonicsCoefficients property to access the generated coefficients.

## See Also

### Working with Spherical Harmonics

var sphericalHarmonicsCoefficients: Data?

Data containing the spherical harmonics coefficients for the light.

var sphericalHarmonicsLevel: Int

The number of levels of spherical harmonics information in the light probe.

