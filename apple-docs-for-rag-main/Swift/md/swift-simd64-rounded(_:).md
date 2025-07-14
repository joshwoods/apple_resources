

- Swift
- SIMD64
-  rounded(\_:) 

Instance Method

# rounded(\_:)

A vector formed by rounding each lane of the source vector to an integral value according to the specified rounding `rule`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rounded(_ rule: FloatingPointRoundingRule) -> Self
```

Available when `Scalar` conforms to `FloatingPoint`.

