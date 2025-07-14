

- GameplayKit
- GKNoiseMap
-  init(\_:) 

Initializer

# init(\_:)

Initializes a noise map by sampling from the specified noise object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
convenience init(_ noise: GKNoise)
```

## Parameters 

`noise`  

The noise object from which to create a noise map.

## Return Value

A new noise map object.

## Discussion

This initializer is equivalent to calling the init(_:size:origin:sampleCount:seamless:) initializer with a size of `1.0 x 1.0`, an origin of `[0, 0]`, a sample grid size of `100 x 100`, and a `seamless` parameter of false.

GKNoiseSource and GKNoise objects are lightweight descriptions of noise generation and processing parameters. When you create a noise map from a noise object, GameplayKit performs the computation described by those objects to create an grid of noise sample values. You can then read those values (or interpolated values at non-integral positions on that grid) with the methods listed in Accessing Noise Values in GKNoiseMap, or use the SKTexture or `SKTileMap` classes to generate texture images or tile maps from the generated noise.

For more information, see GameplayKit Programming Guide.

## See Also

### Creating a Noise Map

init(GKNoise, size: vector_double2, origin: vector_double2, sampleCount: vector_int2, seamless: Bool)

Creates a noise map by sampling from the specified noise object.

convenience init()

Initializes a noise map with a constant noise value of zero throughout.

