

- Accelerate
- vDSP
- vDSP.DCT
-  transform(\_:result:) 

Instance Method

# transform(\_:result:)

Computes an out-of-place single-precision real discrete cosine transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func transform(
    _ vector: U,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## See Also

### Instance Methods

func transform&lt;U>(U) -> [Float]

Returns the single-precision real discrete cosine transform.

