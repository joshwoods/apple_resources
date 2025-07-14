

- Swift
-  pointwiseMin(\_:\_:) 

Function

# pointwiseMin(\_:\_:)

The lanewise minimum of two vectors.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func pointwiseMin(
    _ a: T,
    _ b: T
) -> T where T : SIMD, T.Scalar : Comparable
```

## Discussion

Each element of the result is the minimum of the corresponding elements of the inputs.

## See Also

### Supporting Functions

func all&lt;Storage>(SIMDMask&lt;Storage>) -> Bool

True if every lane of mask is true.

func any&lt;Storage>(SIMDMask&lt;Storage>) -> Bool

True if any lane of mask is true.

func pointwiseMax&lt;T>(T, T) -> T

The lanewise maximum of two vectors.

func pointwiseMax&lt;T>(T, T) -> T

The lanewise maximum of two vectors.

func pointwiseMin&lt;T>(T, T) -> T

The lanewise minimum of two vectors.

