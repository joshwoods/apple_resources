

- PHASE
- PHASEEnvelope
-  domain 

Instance Property

# domain

The range of the envelope’s possible input values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var domain: PHASENumericPair { get }
```

## Discussion

This property is an ordered pair that describes input values along the *x* axis for which the evaluate(x:) function can produce a non-zero output. The first number in the pair is the minimum input value, and the second number in the pair is the maximum input value.

When an envelope graphs volume over time, the framework scales the domain by unitsPerSecond. Likewise, when an envelope graphs volume over distance, the framework scales this property by unitsPerMeter.

## See Also

### Bounding the Input

var range: PHASENumericPair

The bounds of the output value.

