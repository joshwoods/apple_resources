

- Model I/O
- MDLTransformComponent
-  setLocalTransform(\_:forTime:) 

Instance Method

# setLocalTransform(\_:forTime:)

Sets a new local transform matrix for the specified time sample.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional func setLocalTransform(
    _ transform: matrix_float4x4,
    forTime time: TimeInterval
)
```

## Parameters 

`transform`  

The local transformation matrix for the specified time sample.

`time`  

The time sample with which to associate transform information.

## Discussion

Calling this method updates the minimumTime and maximumTime properties to reflect the range of sample values stored in the transform component.

## See Also

### Working with Animated Transforms

var minimumTime: TimeInterval

The timestamp for the first timed data sample in the transform component.

**Required**

var maximumTime: TimeInterval

The timestamp for the last timed data sample in the transform component.

**Required**

func localTransform(atTime: TimeInterval) -> matrix_float4x4

Returns the local transform matrix as of the specified time sample.

