

- Model I/O
- MDLLightProbe
-  sphericalHarmonicsLevel 

Instance Property

# sphericalHarmonicsLevel

The number of levels of spherical harmonics information in the light probe.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var sphericalHarmonicsLevel: Int { get }
```

## Discussion

Each level of spherical harmonics contains more coefficients, and thus affects the layout of the data containing those coefficients. For details, see the sphericalHarmonicsCoefficients property.

## See Also

### Working with Spherical Harmonics

func generateSphericalHarmonics(fromIrradiance: Int)

Generates spherical harmonics information based on the light probe’s irradiance texture.

var sphericalHarmonicsCoefficients: Data?

Data containing the spherical harmonics coefficients for the light.

