

- Swift Charts
-  PrimitivePlottableProtocol 

Protocol

# PrimitivePlottableProtocol

A type that represents the primitive plottable types supported by the framework. Don’t use this type directly.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PrimitivePlottableProtocol : Plottable where Self == Self.PrimitivePlottable
```

## Overview

A primitive plottable type is a numeric type like a Float or UInt32 for quantitative values, Date for temporal values, or String for categorical values.

Primitive plottable types conform to the Plottable protocol.

## Relationships

### Inherits From

- Plottable

