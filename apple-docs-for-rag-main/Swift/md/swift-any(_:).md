

- Swift
-  any(\_:) 

Function

# any(\_:)

True if any lane of mask is true.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func any(_ mask: SIMDMask) -> Bool where Storage : SIMD, Storage.Scalar : FixedWidthInteger, Storage.Scalar : SignedInteger
```

## See Also

### Supporting Functions

func all&lt;Storage>(SIMDMask&lt;Storage>) -> Bool

True if every lane of mask is true.

func pointwiseMax&lt;T>(T, T) -> T

The lanewise maximum of two vectors.

func pointwiseMax&lt;T>(T, T) -> T

The lanewise maximum of two vectors.

func pointwiseMin&lt;T>(T, T) -> T

The lanewise minimum of two vectors.

func pointwiseMin&lt;T>(T, T) -> T

The lanewise minimum of two vectors.

