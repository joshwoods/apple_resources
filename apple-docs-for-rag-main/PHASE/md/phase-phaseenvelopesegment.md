

- PHASE
-  PHASEEnvelopeSegment 

Class

# PHASEEnvelopeSegment

A curved portion of an envelope.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEEnvelopeSegment
```

## Overview

This class specifies a curve that determines the \_y-\_value rate of change over a particular portion of an envelope’s graph. For example, the difference between a PHASECurveType.cubed segment and an PHASECurveType.inverseCubed segment is that they share opposite rates of change; where the cubed curve’s *y* value changes fastest in the segment’s domain, the inverse-cubed curve changes slowest, and vice versa.

## Topics

### Creating a Segment

init(endPoint: simd_double2, curveType: PHASECurveType)

Creates a curved portion of an envelope.

### Shaping a Segment

var curveType: PHASECurveType

A curve along the envelope that shapes the segment.

var endPoint: simd_double2

A point that identifies the end of the segment along the envelope.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Dynamic Sound Control

class PHASEEnvelope

A collection of segments that connect to graph a complex curve over a linear input.

enum PHASECurveType

Options that apply a mathematical function to an input value.

class PHASENumericPair

An ordered pair that defines a bounding box for an envelope.

Playback Parameterization

Change the characteristics of in-flight audio by adjusting its properties at runtime.

