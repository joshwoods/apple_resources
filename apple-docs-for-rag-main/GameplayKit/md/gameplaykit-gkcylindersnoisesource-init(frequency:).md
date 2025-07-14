

- GameplayKit
- GKCylindersNoiseSource
-  init(frequency:) 

Initializer

# init(frequency:)

Initializes a cylinder noise source with the specified frequency.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
init(frequency: Double)
```

## Parameters 

`frequency`  

The initial value for the `frequency` property, which determines the size and spacing of concentric cylinders.

## Return Value

A new noise source.

## Discussion

To make use of this noise source, create a GKNoise object from it (and optionally apply operations to that noise object or combine it with other noise objects). Then create a GKNoiseMap object from your noise object, generating a concrete field of values that you can sample from directly or visualize using the SKTexture or `SKTileMap` class.

## See Also

### Creating a Noise Source

class func cylindersNoise(withFrequency: Double) -> Self

Creates a cylinder noise source with the specified frequency.

