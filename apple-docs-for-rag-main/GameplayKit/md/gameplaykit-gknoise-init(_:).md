

- GameplayKit
- GKNoise
-  init(\_:) 

Initializer

# init(\_:)

Initializes a noise object with the specified noise source.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
convenience init(_ noiseSource: GKNoiseSource)
```

## Parameters 

`noiseSource`  

The noise source defining the style and configuration of noise to generate.

## Return Value

A new noise object.

## Discussion

To sample from the newly created object’s noise field or generate texture images, create a GKNoiseMap object from this noise object. Optionally, before doing so you can apply operations to process or transform the noise field, or combine it with other noise objects, to create a more complex or natural noise pattern. For details, see Applying Operations to Noise Values, Applying Operations that Combine Noise, Applying Operations that Distort Noise, Applying Geometric Transformations, and Creating Noise by Combining Noise in GKNoise.

## See Also

### Creating Noise

init(GKNoiseSource, gradientColors: [NSNumber : UIColor])

Initializes a noise object with the specified noise source, with colors for later use in generating noise textures.

