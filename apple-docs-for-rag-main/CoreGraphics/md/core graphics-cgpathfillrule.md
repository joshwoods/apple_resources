

- Core Graphics
-  CGPathFillRule 

Enumeration

# CGPathFillRule

Rules for determining which regions are interior to a path, used by the fillPath(using:) and clip(using:) methods.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CGPathFillRule
```

## Overview

When filling a path, regions that a fill rule defines as interior to the path are painted. When clipping with a path, regions interior to the path remain visible after clipping.

## Topics

### Enumeration Cases

case evenOdd

A rule that considers a region to be interior to a path based on the number of times it is enclosed by path elements.

case winding

A rule that considers a region to be interior to a path if the winding number for that region is nonzero.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Constants

enum CGTextEncoding

Text encodings for fonts.

