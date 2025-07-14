

- TabularData
- OptionalColumnProtocol
-  -(\_:\_:) 

Operator

# -(\_:\_:)

Generates a column by subtracting each element in an optional column type from the corresponding elements of another.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func - (lhs: Self, rhs: Self) -> Column
```

Available when `WrappedElement` conforms to `AdditiveArithmetic`.

## Parameters 

`lhs`  

An optional column type.

`rhs`  

Another optional column type.

## Return Value

A new column.

## See Also

### Generating an Optional Column by Subtracting Two Columns

func - &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by subtracting each element in an optional column type from the corresponding elements of a column type.

func - &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of an optional column.

