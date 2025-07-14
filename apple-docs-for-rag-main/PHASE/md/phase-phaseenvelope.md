

- PHASE
-  PHASEEnvelope 

Class

# PHASEEnvelope

A collection of segments that connect to graph a complex curve over a linear input.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEEnvelope
```

## Overview

In traditional audio uses, an *envelope* defines a complex graph that determines the volume of audio data over an input duration. PHASE uses envelopes in a similar way. Given a value on the envelope’s input axis, the evaluate(x:) function plots and returns the result on the output axis. The following are possible uses of this class:

- Sound event nodes, such as PHASEBlendNodeDefinition, can shape their volume using an envelope; see addRange(envelope:subtree:).

- Distance models shape sounds with a 3D position using an envelope; see PHASEEnvelopeDistanceModelParameters.

- An envelope can do more than shape audio. To gradually change an envelope’s input value over time, use the PHASEMappedMetaParameterDefinition class, which creates a function with a metaparameter value as input. An app can use the numeric result for any purpose. For example, the x-axis can be distance and the y-axis can be playback rate.

At runtime, PHASE determines whether a particular member of the segments array slopes up or down along the domain depending on the envelope’s particular use case.

### Create an Envelope and Shape its Curve

To use an envelope in your app, define its shape by defining a series of segments. Each segment specifies a curve that collectively connect to form a graph. The following code creates an envelope with a single segment that’s shaped like the lettter *s:*

- Swift
- Objective-C

```
// Create a segments array.
var segments: [PHASEEnvelopeSegment] = []

// Create a single segment with a sigmoid curve to give "ease in, 
//  ease out" movement along the domain. Define an endpoint of (1, 1).
let segment = PHASEEnvelopeSegment(
    endPoint: simd_make_double2(1.0, 1.0), curveType: .sigmoid)

// Add the segment to the array.
segments.append(segment)

// Create the envelope and set the start point to (-1, -1).
let envelope = PHASEEnvelope(startPoint: simd_make_double2(-1.0, -1.0),
    segments: segments)
```

```
// Create a segments array.
NSMutableArray* segments = 
    [NSMutableArray new];

// Create a single segment with a sigmoid curve to give "ease in, 
//  ease out" movement along the domain. Define an endpoint of (1, 1).
PHASEEnvelopeSegment* segment = [[PHASEEnvelopeSegment alloc] 
    initWithEndPoint:simd_make_double2(1.0, 1.0) 
    curveType:PHASECurveTypeSigmoid];

// Add the segment to the array.
[segments addObject:segment];

// Create the envelope and set the start point to (-1, -1).
PHASEEnvelope* envelope = [[PHASEEnvelope alloc] 
    initWithStartPoint:simd_make_double2(-1.0, -1.0) 
    segments:segments];
```

The graph flexes at runtime depending on the source content on which the envelope operates. A PHASEEnvelope doesn’t constrain the evaluate(x:) function’s output to predertermined values. Instead, PHASE applies the envelope’s curves to the source content as a rate of change.

## Topics

### Creating an Envelope

init?(startPoint: simd_double2, segments: [PHASEEnvelopeSegment])

Creates an envelope with a start point and segments.

### Inspecting the Envelope

func evaluate(x: Double) -> Double

Provides the height of the envelope for an input value.

var segments: [PHASEEnvelopeSegment]

An array of the envelope’s segments.

var startPoint: simd_double2

The starting point along the envelope’s duration.

### Bounding the Input

var domain: PHASENumericPair

The range of the envelope’s possible input values.

var range: PHASENumericPair

The bounds of the output value.

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

class PHASEEnvelopeSegment

A curved portion of an envelope.

enum PHASECurveType

Options that apply a mathematical function to an input value.

class PHASENumericPair

An ordered pair that defines a bounding box for an envelope.

Playback Parameterization

Change the characteristics of in-flight audio by adjusting its properties at runtime.

