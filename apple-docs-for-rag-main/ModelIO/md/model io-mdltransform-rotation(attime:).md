

- Model I/O
- MDLTransform
-  rotation(atTime:) 

Instance Method

# rotation(atTime:)

Returns the orientation of the transform relative to its parent coordinate space, as of the specified time sample.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func rotation(atTime time: TimeInterval) -> vector_float3
```

## Parameters 

`time`  

The time sample for which to request information.

## Return Value

The orientation, as a vector of Euler angles in radians, of the transform.

## Discussion

The three components of the rotation vector describe counterclockwise rotation around the corresponding axes. In a coordinate system where the negative z-axis direction is considered “forward”, these components are pitch (rotation about the x-axis), yaw (rotation about the y-axis), and roll (rotation about the z-axis).

Together with the translation, scale, and shear factors, rotation defines the local coordinate space for any object affected by the transform, relative to a parent coordinate space. To work with the complete transform, use the localTransform(atTime:) and setLocalTransform(_:forTime:) methods.

Requesting a sample outside the time range clamps results to the minimumTime or maximumTime sample. Some asset formats support continuous sampling, with interpolation for times between the samples stored in the asset; others are discrete. For an asset with discrete time information, requesting a sample time in between the samples stored in the asset returns data for the immediately preceding time.

## See Also

### Using Factors of an Animated Transform

func translation(atTime: TimeInterval) -> vector_float3

Returns the x-, y-, and z-axis offsets of the transform relative to its parent coordinate space, as of the specified time sample.

func setTranslation(vector_float3, forTime: TimeInterval)

Sets the x-, y-, and z-axis offsets of the transform for the specified time sample.

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

func setMatrix(matrix_float4x4, forTime: TimeInterval)

