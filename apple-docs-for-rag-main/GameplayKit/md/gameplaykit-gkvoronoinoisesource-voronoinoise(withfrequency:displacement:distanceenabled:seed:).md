

- GameplayKit
- GKVoronoiNoiseSource
-  voronoiNoise(withFrequency:displacement:distanceEnabled:seed:) 

Type Method

# voronoiNoise(withFrequency:displacement:distanceEnabled:seed:)

Creates a Voronoi noise source with the specified parameters.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class func voronoiNoise(
    withFrequency frequency: Double,
    displacement: Double,
    distanceEnabled: Bool,
    seed: Int32
) -> Self
```

## Parameters 

`frequency`  

The initial value for the frequency property, which determines the number and spacing of cells in generated noise.

`displacement`  

The initial value for the displacement property, which determines the variety of noise values between cells in generated noise.

`distanceEnabled`  

The initial value for the isDistanceEnabled property, which determines whether to add distance values to generated noise.

`seed`  

The initial value for the seed property, which determines the overall structure of generated noise.

## Return Value

A new noise source.

## Discussion

To make use of this noise source, create a GKNoise object from it (and optionally apply operations to that noise object or combine it with other noise objects). Then create a GKNoiseMap object from your noise object, generating a concrete field of values that you can sample from directly or visualize using the SKTexture or `SKTileMap` class.

## See Also

### Creating a Noise Source

init(frequency: Double, displacement: Double, distanceEnabled: Bool, seed: Int32)

Initializes a Voronoi noise source with the specified parameters.

