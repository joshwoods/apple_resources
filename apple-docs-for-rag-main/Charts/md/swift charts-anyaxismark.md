

- Swift Charts
-  AnyAxisMark 

Structure

# AnyAxisMark

A type-erased axis mark.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct AnyAxisMark
```

## Topics

### Initializers

init(any AxisMark)

init(erasing: some AxisMark)

## Relationships

### Conforms To

- AxisMark

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

struct AxisValue

A value for an axis mark.

struct AxisMarkBuilder

A result builder that constructs axis marks and overrides default marks.

