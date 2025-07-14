

- Model I/O
- MDLTransformComponent
-  matrix 

Instance Property

# matrix

The transform matrix that defines the local coordinate space relative to a parent coordinate space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var matrix: matrix_float4x4 { get set }
```

**Required**

## Discussion

This matrix defines the position, orientation, shear, and scale for any object affected by the transform component, relative to the coordinate space of its parent.

If the transform component includes time-based transform information, this method returns the local transform matrix as of the earliest time sample (as reported by the minimumTime property).

## See Also

### Working with Static Transforms

func setLocalTransform(matrix_float4x4)

Sets a new static transform matrix, overriding any time-based transform information.

