

- Accelerate
- vDSP
- vDSP.DCT
-  transform(\_:) 

Instance Method

# transform(\_:)

Returns the single-precision real discrete cosine transform.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func transform(_ vector: U) -> [Float] where U : AccelerateBuffer, U.Element == Float
```

## See Also

### Instance Methods

func transform&lt;U, V>(U, result: inout V)

Computes an out-of-place single-precision real discrete cosine transform.

