

- TabularData
- Column
-  \*=(\_:\_:) 

Operator

# \*=(\_:\_:)

Modifies a column by multiplying each element in the column by the corresponding value in a collection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func *= (lhs: inout Column, rhs: C) where WrappedElement : Numeric, WrappedElement == C.Element, C : Collection
```

## Parameters 

`lhs`  

A column.

`rhs`  

A collection that contains elements of the same type as the column’s elements.

## See Also

### Modifying a Column with a Collection of Values

static func += &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by adding each value in a collection to the corresponding element in the column.

static func += &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by adding each optional value in a collection to the corresponding element in the column.

static func -= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by subtracting each value in a collection from the corresponding element in the column.

static func -= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by subtracting each optional value in a collection from the corresponding element in the column.

static func *= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by multiplying each element in the column by the corresponding optional value in a collection.

static func /= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies an integer column by dividing each element in the column by the corresponding value in a collection.

static func /= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies an integer column by dividing each element in the column by the corresponding optional value in a collection.

static func /= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a floating-point column by dividing each element in the column by the corresponding value in a collection.

static func /= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a floating-point column by dividing each element in the column by the corresponding optional value in a collection.

