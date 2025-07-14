

- PHASE
-  PHASENumericPair 

Class

# PHASENumericPair

An ordered pair that defines a bounding box for an envelope.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASENumericPair
```

## Overview

A PHASEEnvelope object uses this class to bound the value of its range and domain.

## Topics

### Creating a Numeric Pair

init(firstValue: Double, secondValue: Double)

Creates a pair of numbers with the given values.

### Defining the Values

var first: Double

The first value in the pair.

var second: Double

The second value in the pair.

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

class PHASEEnvelopeSegment

A curved portion of an envelope.

enum PHASECurveType

Options that apply a mathematical function to an input value.

Playback Parameterization

Change the characteristics of in-flight audio by adjusting its properties at runtime.

