

- PHASE
-  PHASECurveType 

Enumeration

# PHASECurveType

Options that apply a mathematical function to an input value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASECurveType
```

## Overview

PHASE applies curves in several places across the framework:

- A PHASEEnvelopeSegment object represents one curved portion of an envelope’s graph.

- The PHASEGroup class applies a curve type to its sounds by fading its volume with the fadeGain(gain:duration:curveType:) function, and to its rate, with fadeRate(rate:duration:curveType:).

- Each PHASEGroupPresetSetting applies a curve to control a setting’s rate of change.

### Apply a Curve as a Rate of Change

In most cases, PHASE applies curves to output a rate of change. For example, an envelope segment’s curveType determines where along the segment’s domain the y-value changes more quickly. The following figure compares all the curves’ rate of change by plotting their input over the range `(0,0)` to `(1,1)`.

## Topics

### Types

case linear

A curve that increases uniformly with its input.

case squared

A curve that increases at a rate that squares its input.

case inverseSquared

A curve that increases at a rate of one divided by the input’s square.

case cubed

A curve that increases at a rate that cubes its input.

case inverseCubed

A curve that increases at a rate of one divided by the input’s cube.

case sine

A sine curve.

case inverseSine

An inverse sine curve.

case sigmoid

A sigmoid curve.

case inverseSigmoid

An inverse sigmoid curve.

case holdStartValue

A curve that equals its start value for the entire duration.

case jumpToEndValue

A curve that equals its end value for the entire duration.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Dynamic Sound Control

class PHASEEnvelope

A collection of segments that connect to graph a complex curve over a linear input.

class PHASEEnvelopeSegment

A curved portion of an envelope.

class PHASENumericPair

An ordered pair that defines a bounding box for an envelope.

Playback Parameterization

Change the characteristics of in-flight audio by adjusting its properties at runtime.

