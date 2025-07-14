

- TabularData
- FilledColumn
-  \>(\_:\_:) 

Operator

# \>(\_:\_:)

Returns a Boolean array that indicates whether the corresponding element of a column type is greater than a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func > (lhs: Self, rhs: Self.Element) -> [Bool]
```

Available when `Element` conforms to `Comparable`.

## Return Value

A Boolean array.

## Discussion

- lhs: A column type.

- rhs: A value of the same type as the column.

