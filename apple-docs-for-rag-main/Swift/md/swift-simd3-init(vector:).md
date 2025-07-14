

- Swift
- SIMD3
-  init(vector:) 

Initializer

# init(vector:)

Returns a new vector from a Spatial point.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+Mac Catalyst 16.0+

``` source
init(vector: Vector3D)
```

Available when `Scalar` is `Float`.

## Discussion

Values rounded to a representable value, if necessary.

Note

This function is provided as a convenience. All Spatial storage and calculations are double-precision.

