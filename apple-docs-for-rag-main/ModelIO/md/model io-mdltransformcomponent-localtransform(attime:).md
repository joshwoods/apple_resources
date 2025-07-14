

- Model I/O
- MDLTransformComponent
-  localTransform(atTime:) 

Instance Method

# localTransform(atTime:)

Returns the local transform matrix as of the specified time sample.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional func localTransform(atTime time: TimeInterval) -> matrix_float4x4
```

## Parameters 

`time`  

The time sample for which to request information.

## Return Value

The local transformation matrix for the specified time sample.

## Discussion

This matrix defines the position, orientation, shear, and scale for any object affected by the transform component, relative to the coordinate space of its parent, as of the specified time sample.

Requesting a sample outside the time range clamps returned values using the minimumTime and maximumTime properties. Some asset formats support continuous sampling, with interpolation for times between the samples stored in the asset; others are discrete. For an asset with discrete time information, requesting a sample time in between the samples stored in the asset returns data for the immediately preceding time.

## See Also

### Working with Animated Transforms

var minimumTime: TimeInterval

The timestamp for the first timed data sample in the transform component.

**Required**

var maximumTime: TimeInterval

The timestamp for the last timed data sample in the transform component.

**Required**

func setLocalTransform(matrix_float4x4, forTime: TimeInterval)

Sets a new local transform matrix for the specified time sample.

