

- GameplayKit
- GKNoiseMap
-  init(\_:size:origin:sampleCount:seamless:) 

Initializer

# init(\_:size:origin:sampleCount:seamless:)

Creates a noise map by sampling from the specified noise object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
init(
    _ noise: GKNoise,
    size: vector_double2,
    origin: vector_double2,
    sampleCount: vector_int2,
    seamless: Bool
)
```

## Parameters 

`noise`  

The noise object from which GKNoiseMap samples data.

`size`  

The size is the width and height of a 2-dimensional plane within the noise grid of the GKNoise object.

`origin`  

The start position of the noise samples within the 2-dimensional plane of the noise as defined by the size parameter. This value needs to be within the range of 0 and the size parameter.

`sampleCount`  

The number of samples in the x and y dimensions of the 2D noise plane starting at the origin up to the size parameter.

If an SKTexture image is generated the width and height of the SKTexture corresponds to the sampleCount width and height.

`seamless`  

A Boolean value that when true indicates the system adjusts samples from the noise object so that generated texture images can tile without visible seams.

## Return Value

A new noise map object.

## Discussion

GKNoiseSource and GKNoise objects are lightweight descriptions of noise generation and processing parameters. When you create a noise map from a noise object, GameplayKit performs the computation described by those objects to create a grid of noise sample values. You can then read those values (or interpolated values at non-integral positions on that grid) with the methods listed in Accessing Noise Values, or use the SKTexture or `SKTileMap` classes to generate texture images or tile maps from the generated noise.

The noise field described by a GKNoise object is inherently three-dimensional and infinite in extent. When you create a noise map from a noise object, GameplayKit samples a “slice” of noise values, whose size and position within the `z = 0` plane of the noise field you specify with the `size` and `origin` parameters. You can take advantage of these features by using GKNoise methods to rotate, translate, and scale the noise field before creating a noise map:

- Generate wood-grain textures by creating and distorting GKCylindersNoiseSource output, then rotating it to “slice” diagonally along the cylinders.

- Use one of the GKCoherentNoiseSource classes as the basis for an infinite procedurally-generated game world by translating the noise field, then generating noise maps for areas of the world near the player. Because coherent noise is deterministic, you can discard noise maps when the player leaves an area, and regenerate them when the player comes back.

## See Also

### Creating a Noise Map

convenience init(GKNoise)

Initializes a noise map by sampling from the specified noise object.

convenience init()

Initializes a noise map with a constant noise value of zero throughout.

