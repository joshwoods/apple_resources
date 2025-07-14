

- Model I/O
- MDLLightProbeIrradianceDataSource
-  boundingBox 

Instance Property

# boundingBox

The bounding region of the scene to which light probes are being added.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var boundingBox: MDLAxisAlignedBoundingBox { get set }
```

**Required**

## Discussion

When you call the MDLAsset placeLightProbes(withDensity:heuristic:using:) method to automatically distribute light probes in a scene, Model I/O reads this property to ask your code which regions should be evaluated for light probe placement.

## See Also

### Providing Light Probe Information

var sphericalHarmonicsLevel: Int

The number of levels of spherical harmonics information provided by the data source.

func sphericalHarmonicsCoefficients(atPosition: vector_float3) -> Data

Asks the data source to provide spherical harmonics coefficients that describe lighting conditions in all directions from the specified point in a scene.

