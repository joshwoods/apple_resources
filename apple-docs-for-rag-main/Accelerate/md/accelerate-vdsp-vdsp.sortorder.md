

- Accelerate
- vDSP
-  vDSP.SortOrder 

Enumeration

# vDSP.SortOrder

Constants that specify the sorting order.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum SortOrder
```

## Topics

### Enumeration Cases

case ascending

An ascending search.

case descending

A descending search.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Vector sorting functions

static func sort&lt;V>(inout V, sortOrder: vDSP.SortOrder)

Sorts a vector of single-precision values in-place.

static func sort&lt;V>(inout V, sortOrder: vDSP.SortOrder)

Sorts a vector of double-precision values in-place.

