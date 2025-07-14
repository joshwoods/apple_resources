

- Accelerate
- vDSP
-  integrate(\_:using:stepSize:result:) 

Type Method

# integrate(\_:using:stepSize:result:)

Performs the integration of a single-precision using the specified rule.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func integrate(
    _ vector: U,
    using rule: vDSP.IntegrationRule,
    stepSize: Float = 1,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## See Also

### Integration

static func integrate&lt;U>(U, using: vDSP.IntegrationRule, stepSize: Double) -> [Double]

Returns the integration of a double-precision vector using the specified rule.

static func integrate&lt;U>(U, using: vDSP.IntegrationRule, stepSize: Float) -> [Float]

Returns the integration of a single-precision vector using the specified rule.

static func integrate&lt;U, V>(U, using: vDSP.IntegrationRule, stepSize: Double, result: inout V)

Performs the integration of a double-precision using the specified rule.

enum IntegrationRule

Integration rules.

