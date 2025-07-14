

- Model I/O
- MDLPhotometricLight
-  sphericalHarmonicsLevel 

Instance Property

# sphericalHarmonicsLevel

The number of levels of generated spherical harmonics information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var sphericalHarmonicsLevel: Int { get }
```

## Discussion

Each level of spherical harmonics contains more coefficients, and thus affects the layout of the data containing those coefficients. For details, see the sphericalHarmonicsCoefficients property.

## See Also

### Interpreting the Light Web as Spherical Harmonics

func generateSphericalHarmonics(fromLight: Int)

Generates spherical harmonics information based on the light’s photometry data.

var sphericalHarmonicsCoefficients: Data?

Data containing spherical harmonics coefficients that describe the light’s intensity in all directions.

