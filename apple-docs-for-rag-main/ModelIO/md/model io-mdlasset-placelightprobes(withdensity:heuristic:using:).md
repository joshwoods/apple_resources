

- Model I/O
- MDLAsset
-  placeLightProbes(withDensity:heuristic:using:) 

Type Method

# placeLightProbes(withDensity:heuristic:using:)

Automatically creates and places light probes for use in illuminating a scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func placeLightProbes(
    withDensity value: Float,
    heuristic type: MDLProbePlacement,
    using dataSource: any MDLLightProbeIrradianceDataSource
) -> [MDLLightProbe]
```

## Parameters 

`value`  

A value that determines the coarseness or fineness with which to evaluate the scene. Lower values evaluate fewer positions, resulting in fewer light probes and lower fidelity. Higher values evaluate more positions, resulting in higher fidelity at increased computational cost.

`type`  

An option that determine how Model I/O uses the data source to position light probes.

`dataSource`  

A custom object that provides information about the scene to be evaluated.

## Return Value

An array of light probe objects for use in the scene.

## Discussion

When you call this method, you must pass a custom object implementing the MDLLightProbeIrradianceDataSource protocol. Model I/O queries this object to determine how to place light probes.

When you use the MDLProbePlacement.uniformGrid heuristic, Model I/O simply divides the boundingBox region your data source provides into `value` units in each dimension, and creates an array of light probe objects to fill each position in the resulting grid.

When you use the MDLProbePlacement.irradianceDistribution heuristic, Model I/O uses the same grid to sample information about the lighting conditions in your scene (by calling the sphericalHarmonicsLevel and sphericalHarmonicsCoefficients(atPosition:) methods of your data source), then creates and positions light probes to optimally account for differences in lighting conditions across the scene.

## See Also

### Working with Lights

enum MDLProbePlacement

Options affecting automatic placement of light probes in a scene, used with the placeLightProbes(withDensity:heuristic:using:) method.

