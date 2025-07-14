

- Model I/O
- MDLTransform
-  setMatrix(\_:forTime:) 

Instance Method

# setMatrix(\_:forTime:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func setMatrix(
    _ matrix: matrix_float4x4,
    forTime time: TimeInterval
)
```

## See Also

### Using Factors of an Animated Transform

func translation(atTime: TimeInterval) -> vector_float3

Returns the x-, y-, and z-axis offsets of the transform relative to its parent coordinate space, as of the specified time sample.

func setTranslation(vector_float3, forTime: TimeInterval)

Sets the x-, y-, and z-axis offsets of the transform for the specified time sample.

func rotation(atTime: TimeInterval) -> vector_float3

Returns the orientation of the transform relative to its parent coordinate space, as of the specified time sample.

func rotationMatrix(atTime: TimeInterval) -> matrix_float4x4

Returns the orientation of the transform as a rotation matrix, as of the specified time sample.

func setRotation(vector_float3, forTime: TimeInterval)

Sets the orientation of the transform for the specified time sample.

func scale(atTime: TimeInterval) -> vector_float3

Returns the x-, y-, and z-axis scale factors of the transform relative to its parent coordinate space, as of the specified time sample.

func setScale(vector_float3, forTime: TimeInterval)

Sets the x-, y-, and z-axis scale factors of the transform for the specified time sample.

func shear(atTime: TimeInterval) -> vector_float3

Returns the x-, y-, and z-axis shear factors of the transform relative to its parent coordinate space, as of the specified time sample.

func setShear(vector_float3, forTime: TimeInterval)

Sets the x-, y-, and z-axis shear factors of the transform for the specified time sample.

