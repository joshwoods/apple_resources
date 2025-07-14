

- GameplayKit
- GKNoiseMap
-  origin 

Instance Property

# origin

The position of the “slice” of noise samples contained in the noise map relative to the unit coordinate space of the noise object it was created from.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var origin: vector_double2 { get }
```

## Discussion

This property is read-only; you define the origin of a noise map when creating it with the interpolatedValue(at:) initializer.

## See Also

### Inspecting a Noise Map

var size: vector_double2

The size of the “slice” of noise samples contained in the noise map relative to the unit coordinate space of the noise object it was created from.

var sampleCount: vector_int2

The width and height of integer grid for which the noise map contains sampled noise values.

var isSeamless: Bool

A Boolean value indicating whether the noise map’s output can repeat seamlessly in all directions.

