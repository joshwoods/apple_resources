

- TabularData
- DiscontiguousColumnSlice
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean that indicates whether the column slices are equal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func == (lhs: DiscontiguousColumnSlice, rhs: DiscontiguousColumnSlice) -> Bool
```

Available when `WrappedElement` conforms to `Equatable`.

## Parameters 

`lhs`  

A discontiguous column slice.

`rhs`  

Another discontiguous column slice.

## See Also

### Comparing Two Column Slices

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

