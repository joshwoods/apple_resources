

- PHASE
- PHASEEnvelope
-  startPoint 

Instance Property

# startPoint

The starting point along the envelope’s duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var startPoint: simd_double2 { get }
```

## Discussion

The framework sets the value of this property to the init(startPoint:segments:) argument.

## See Also

### Inspecting the Envelope

func evaluate(x: Double) -> Double

Provides the height of the envelope for an input value.

var segments: [PHASEEnvelopeSegment]

An array of the envelope’s segments.

