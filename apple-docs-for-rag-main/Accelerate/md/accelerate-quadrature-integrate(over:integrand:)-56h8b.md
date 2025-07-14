

- Accelerate
- Quadrature
-  integrate(over:integrand:) 

Instance Method

# integrate(over:integrand:)

Performs the integration over the supplied vector function.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func integrate(
    over interval: ClosedRange,
    integrand: (UnsafeBufferPointer, UnsafeMutableBufferPointer) -> ()
) -> Result
```

## See Also

### Instance Methods

func integrate(over: ClosedRange&lt;Double>, integrand: (Double) -> Double) -> Result&lt;(integralResult: Double, estimatedAbsoluteError: Double), Quadrature.Error>

Performs the integration over the supplied scalar function.

