

- TabularData
- FilledColumn
-  \>=(\_:\_:) 

Operator

# \>=(\_:\_:)

Returns a Boolean array that indicates whether the value is greater than or equal to the corresponding element of a column type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func >= (lhs: Self.Element, rhs: Self) -> [Bool]
```

Available when `Element` conforms to `Comparable`.

## Return Value

A Boolean array.

## Discussion

- lhs: A value of the same type as the column.

- rhs: A column type.

