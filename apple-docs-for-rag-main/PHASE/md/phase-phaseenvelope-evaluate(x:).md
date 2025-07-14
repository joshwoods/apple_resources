

- PHASE
- PHASEEnvelope
-  evaluate(x:) 

Instance Method

# evaluate(x:)

Provides the height of the envelope for an input value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func evaluate(x: Double) -> Double
```

## Parameters 

`x`  

A value within the envelope’s domain. The envelope clamps this parameter to a value within domain.

## Return Value

The curve’s height for the argument *x* value.

## See Also

### Inspecting the Envelope

var segments: [PHASEEnvelopeSegment]

An array of the envelope’s segments.

var startPoint: simd_double2

The starting point along the envelope’s duration.

