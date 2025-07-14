

- TabularData
- FilledColumn
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean array that indicates whether the corresponding element of a column type is equal to a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func == (lhs: Self, rhs: Self.Element) -> [Bool]
```

Available when `Element` conforms to `Comparable`.

## Return Value

A Boolean array.

## Discussion

- lhs: A column type.

- rhs: A value of the same type as the column.

## See Also

### Comparing a Column with a Value

static func == (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is equal to the corresponding element of a column type.

static func != (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type isn’t equal to a value.

static func != (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value isn’t equal to the corresponding element of a column type.

