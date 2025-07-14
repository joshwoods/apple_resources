

- Model I/O
- MDLLightProbe
-  sphericalHarmonicsCoefficients 

Instance Property

# sphericalHarmonicsCoefficients

Data containing the spherical harmonics coefficients for the light.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var sphericalHarmonicsCoefficients: Data? { get }
```

## Discussion

Spherical harmonic coefficients describe the distribution of light around a light source with less high-frequency detail than a cube map texture, but they can be used more efficiently in real-time rendering. Use the generateSphericalHarmonics(fromIrradiance:) method to create spherical harmonics data based on the light probe’s irradiance texture.

The data is an array of 32-bit floating-point values, containing three noninterleaved data sets corresponding to the red, green, and blue sets of coefficients. The array’s length is determined by the sphericalHarmonicsLevel property:

- At level 0, the array has 1 coefficient (3 values).

- At level 1, the array has 4 coefficients (3 sets of 4 values, 12 values total).

- At level 2, the array has 9 coefficients (3 sets of 9 values, 27 values total).

- At level 3, the array has 16 coefficients (3 sets of 16 values, 48 values total).

- Spherical harmonics levels beyond 3 are not supported.

For example, the code below shows how to access the second coefficient at level 2.

- Swift
- Objective-C

```
```

```
float numberOfCoefficients(int level) {
    return (level + 1) * (level + 1)
}
float offsetForLevel(int level) {
    return numberOfCoefficients(level - 1) - 1
}
float *coeffs = (float *)lightProbe.sphericalHarmonicsCoefficients.bytes;
int totalCount = numberOfCoefficients(lightProbe.sphericalHarmonicsLevel);
int offset = offsetForLevel(2); // level 2 has 3 sets of coefficients, at indexes 3, 4, and 5
int index = 1; // get the second of 3 coefficients on level 2 (zero-based index)
float red = coeffs[offset + index];
float green = coeffs[totalCount + offset + index];
float blue = coeffs[totalCount * 2 + offset + index];
```

## See Also

### Working with Spherical Harmonics

func generateSphericalHarmonics(fromIrradiance: Int)

Generates spherical harmonics information based on the light probe’s irradiance texture.

var sphericalHarmonicsLevel: Int

The number of levels of spherical harmonics information in the light probe.

