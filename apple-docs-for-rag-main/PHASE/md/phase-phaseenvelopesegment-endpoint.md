

- PHASE
- PHASEEnvelopeSegment
-  endPoint 

Instance Property

# endPoint

A point that identifies the end of the segment along the envelope.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var endPoint: simd_double2 { get set }
```

## Discussion

The framework connects this property to the prior segment’s end point, or the envelope startPoint, in the case of the first segment.

## See Also

### Shaping a Segment

var curveType: PHASECurveType

A curve along the envelope that shapes the segment.

