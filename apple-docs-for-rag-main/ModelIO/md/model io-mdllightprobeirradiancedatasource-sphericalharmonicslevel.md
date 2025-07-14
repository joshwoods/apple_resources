

- Model I/O
- MDLLightProbeIrradianceDataSource
-  sphericalHarmonicsLevel 

Instance Property

# sphericalHarmonicsLevel

The number of levels of spherical harmonics information provided by the data source.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional var sphericalHarmonicsLevel: Int { get set }
```

## Discussion

Each level of spherical harmonics contains more coefficients, and thus affects the layout of the data containing those coefficients. For details, see the sphericalHarmonicsCoefficients(atPosition:) method.

## See Also

### Providing Light Probe Information

var boundingBox: MDLAxisAlignedBoundingBox

The bounding region of the scene to which light probes are being added.

**Required**

func sphericalHarmonicsCoefficients(atPosition: vector_float3) -> Data

Asks the data source to provide spherical harmonics coefficients that describe lighting conditions in all directions from the specified point in a scene.

