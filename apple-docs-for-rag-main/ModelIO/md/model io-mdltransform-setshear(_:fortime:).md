

- Model I/O
- MDLTransform
-  setShear(\_:forTime:) 

Instance Method

# setShear(\_:forTime:)

Sets the x-, y-, and z-axis shear factors of the transform for the specified time sample.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setShear(
    _ shear: vector_float3,
    forTime time: TimeInterval
)
```

## Parameters 

`shear`  

The shear factors to set for the transform relative to its parent coordinate space.

`time`  

The time sample with which to associate transform information.

## Discussion

Together with the translation, rotation, and scale factors, a shear vector defines the local coordinate space for any object affected by the transform, relative to a parent coordinate space. To work with the complete transform, use the localTransform(atTime:) and setLocalTransform(_:forTime:) methods.

Setting a new shear synthesizes a complete transform matrix by combining the new translation with the translation(atTime:), rotation(atTime:), and scale(atTime:) factors for the specified time. If the new time is outside the range of the minimumTime and maximumTime properties, this method updates those values to reflect the range of time samples stored in the transform object.

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

func setMatrix(matrix_float4x4, forTime: TimeInterval)

