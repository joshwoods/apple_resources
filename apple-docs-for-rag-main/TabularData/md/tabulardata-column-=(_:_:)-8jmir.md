

- TabularData
- Column
-  /=(\_:\_:) 

Operator

# /=(\_:\_:)

Modifies an integer column by dividing each element by a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func /= (lhs: inout Column, rhs: WrappedElement) where WrappedElement : BinaryInteger
```

## Parameters 

`lhs`  

A column.

`rhs`  

A value of the same type as the column’s elements.

## See Also

### Modifying a Column with a Value

static func += (inout Column&lt;WrappedElement>, WrappedElement)

Modifies a column by adding a value to each element.

static func -= (inout Column&lt;WrappedElement>, WrappedElement)

Modifies a column by subtracting a value from each element.

static func *= (inout Column&lt;WrappedElement>, WrappedElement)

Modifies a column by multiplying each element by a value.

static func /= (inout Column&lt;WrappedElement>, WrappedElement)

Modifies a floating-point column by dividing each element by a value.

