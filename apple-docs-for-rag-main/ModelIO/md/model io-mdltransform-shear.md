

- Model I/O
- MDLTransform
-  shear 

Instance Property

# shear

The x-, y-, and z-axis shear factors of the transform relative to its parent coordinate space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var shear: vector_float3 { get set }
```

## Discussion

Together with the translation, rotation, and scale properties, this property defines the local coordinate space for any object affected by the transform, relative to a parent coordinate space. Use the matrix property to work with the complete transform.

If the transform includes time-based information, reading this property returns the scale as of the earliest time sample (as reported by the minimumTime property). Writing to this property erases any time-sampled data for the scale factor. To work with time-sampled data from an animated transform, use the scale(atTime:) and setScale(_:forTime:) methods.

## See Also

### Using Factors of a Static Transform

var translation: vector_float3

The x-, y-, and z-axis offsets of the transform relative to its parent coordinate space.

var rotation: vector_float3

The orientation, as a vector of Euler angles in radians, of the transform relative to its parent coordinate space.

var scale: vector_float3

The x-, y-, and z-axis scale factors of the transform relative to its parent coordinate space.

func setIdentity()

Sets all factors of the transform to those of the identity transformation.

