

- PHASE
- PHASEEnvelope
-  range 

Instance Property

# range

The bounds of the output value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var range: PHASENumericPair { get }
```

## Discussion

This property is an ordered pair that defines the range of possible output values along the *y* axis for the evaluate(x:) function. The first number in the pair is the minimum output value, and the second number in the pair is the maximum output value.

## See Also

### Bounding the Input

var domain: PHASENumericPair

The range of the envelope’s possible input values.

