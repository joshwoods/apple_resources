

- Swift Charts
-  AxisValue 

Structure

# AxisValue

A value for an axis mark.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AxisValue
```

## Topics

### Instance Properties

var count: Int

The number of values on this axis.

var index: Int

The index of the value along the axis.

### Instance Methods

func `as`&lt;P>(P.Type) -> P?

## Relationships

### Conforms To

- Sendable

## See Also

### Axis marks

protocol AxisMark

A type that serves as the basic building block for the elements of an axis.

struct AxisTick

A mark that a chart draws on an axis to indicate a reference point along that axis.

struct AxisGridLine

A line that a chart draws across its plot area to indicate a reference point along a particular axis.

struct AxisValueLabel

A label that describes the value for an axis mark.

struct AnyAxisMark

A type-erased axis mark.

struct AxisMarkBuilder

A result builder that constructs axis marks and overrides default marks.

