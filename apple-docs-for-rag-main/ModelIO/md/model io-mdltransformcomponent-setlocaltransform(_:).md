

- Model I/O
- MDLTransformComponent
-  setLocalTransform(\_:) 

Instance Method

# setLocalTransform(\_:)

Sets a new static transform matrix, overriding any time-based transform information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional func setLocalTransform(_ transform: matrix_float4x4)
```

## Parameters 

`transform`  

A new static transform matrix.

## Discussion

Calling this method sets both the minimumTime and maximumTime properties to zero.

## See Also

### Working with Static Transforms

var matrix: matrix_float4x4

The transform matrix that defines the local coordinate space relative to a parent coordinate space.

**Required**

