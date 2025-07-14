

- GameplayKit
- GKNoiseMap
-  setValue(\_:at:) 

Instance Method

# setValue(\_:at:)

Sets the value at the specified position in the noise map.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setValue(
    _ value: Float,
    at position: vector_int2
)
```

## Parameters 

`value`  

The new value to set.

`position`  

A position in the noise map’s integer grid.

## Discussion

## See Also

### Accessing Noise Values

func value(at: vector_int2) -> Float

Returns the value at the specified position in the noise map’s discrete sample grid.

func interpolatedValue(at: vector_float2) -> Float

Returns the value at the specified position in the noise map, interpolating results for positions not on the discrete sample grid.

