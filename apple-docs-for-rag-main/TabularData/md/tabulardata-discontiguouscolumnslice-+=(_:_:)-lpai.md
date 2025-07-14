

- TabularData
- DiscontiguousColumnSlice
-  +=(\_:\_:) 

Operator

# +=(\_:\_:)

Modifies a column slice by adding each optional value in a collection to the corresponding element in the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func += (lhs: inout DiscontiguousColumnSlice, rhs: C) where WrappedElement : AdditiveArithmetic, C : Collection, C.Element == WrappedElement?
```

## Parameters 

`lhs`  

A column.

`rhs`  

A collection that contains elements of the same type as the column’s elements.

## See Also

### Modifying a Column Slice with a Collection of Values

static func += &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by adding each value in a collection to the corresponding element in the column.

static func -= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by subtracting each value in a collection from the corresponding element in the column.

static func -= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by subtracting each optional value in a collection from the corresponding element in the column.

static func *= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by multiplying each element in the column by the corresponding value in a collection.

static func *= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by multiplying each element in the column by the corresponding optional value in a collection.

static func /= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies an integer column slice by dividing each element in the column by the corresponding value in a collection.

static func /= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies an integer column slice by dividing each element in the column by the corresponding optional value in a collection.

static func /= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a floating-point column slice by dividing each element in the column by the corresponding value in a collection.

static func /= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a floating-point column slice by dividing each element in the column by the corresponding optional value in a collection.

