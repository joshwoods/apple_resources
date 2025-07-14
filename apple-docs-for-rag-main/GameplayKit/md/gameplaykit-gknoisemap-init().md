

- GameplayKit
- GKNoiseMap
-  init() 

Initializer

# init()

Initializes a noise map with a constant noise value of zero throughout.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
convenience init()
```

## Return Value

A new noise map object.

## Discussion

This convenience initializer is equivalent to creating a GKNoise object from GKConstantNoiseSource output with a constant value of zero, then using the init(_:) initializer to create a noise map from the result.

## See Also

### Creating a Noise Map

convenience init(GKNoise)

Initializes a noise map by sampling from the specified noise object.

init(GKNoise, size: vector_double2, origin: vector_double2, sampleCount: vector_int2, seamless: Bool)

Creates a noise map by sampling from the specified noise object.

