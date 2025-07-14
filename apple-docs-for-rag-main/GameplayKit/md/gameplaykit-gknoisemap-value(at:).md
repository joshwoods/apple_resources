

- GameplayKit
- GKNoiseMap
-  value(at:) 

Instance Method

# value(at:)

Returns the value at the specified position in the noise map’s discrete sample grid.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func value(at position: vector_int2) -> Float
```

## Parameters 

`position`  

The position to query in the noise map’s grid of sampled noise values. Must be within the rectangle from `[0, 0]` to the noise map’s sampleCount value.

## Return Value

The value at the specified position.

## Discussion

When you create a noise map from a GKNoise object, GameplayKit performs the noise generation and processing computations necessary to fill a discrete grid with noise samples. (You specify the size of the grid and its number of samples in the init(_:size:origin:sampleCount:seamless:) initializer.) Use this method to get sample values from that grid.

You can also use the interpolatedValue(at:) method to query positions that are not on the discrete integer grid of samples.

## See Also

### Accessing Noise Values

func interpolatedValue(at: vector_float2) -> Float

Returns the value at the specified position in the noise map, interpolating results for positions not on the discrete sample grid.

func setValue(Float, at: vector_int2)

Sets the value at the specified position in the noise map.

