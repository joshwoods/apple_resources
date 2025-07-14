

- Spatial
- ProjectiveTransform3D
-  isApproximatelyEqual(to:tolerance:) 

Instance Method

# isApproximatelyEqual(to:tolerance:)

Returns a Boolean value that indicates whether two transforms are equal within a specified tolerance.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func isApproximatelyEqual(
    to other: ProjectiveTransform3D,
    tolerance: Double = sqrt(.ulpOfOne)
) -> Bool
```

## Parameters 

`other`  

The right-hand side value.

`tolerance`  

A double-precision value that specifies the tolerance.

