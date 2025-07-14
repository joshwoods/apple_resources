

- Accelerate
- vDSP
-  limit(\_:limit:withOutputConstant:result:) 

Type Method

# limit(\_:limit:withOutputConstant:result:)

Calculates the single-precision vector test limit.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func limit(
    _ vector: U,
    limit: Float,
    withOutputConstant outputConstant: Float,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## See Also

### Limit Operations

static func limit&lt;U>(U, limit: Double, withOutputConstant: Double) -> [Double]

Returns the double-precision vector test limit.

static func limit&lt;U>(U, limit: Float, withOutputConstant: Float) -> [Float]

Returns the single-precision vector test limit.

static func limit&lt;U, V>(U, limit: Double, withOutputConstant: Double, result: inout V)

Calculates the double-precision vector test limit.

