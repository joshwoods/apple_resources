

- Model I/O
- MDLTransformComponent
-  maximumTime 

Instance Property

# maximumTime

The timestamp for the last timed data sample in the transform component.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var maximumTime: TimeInterval { get }
```

**Required**

## Discussion

Timed data is clamped to the minimum and maximum times. If you request transform data for a time sample after the maximum time, Model I/O returns the transform at the maximum time.

If the transform component does not contain timed information, this property’s value is zero.

## See Also

### Working with Animated Transforms

var minimumTime: TimeInterval

The timestamp for the first timed data sample in the transform component.

**Required**

func localTransform(atTime: TimeInterval) -> matrix_float4x4

Returns the local transform matrix as of the specified time sample.

func setLocalTransform(matrix_float4x4, forTime: TimeInterval)

Sets a new local transform matrix for the specified time sample.

