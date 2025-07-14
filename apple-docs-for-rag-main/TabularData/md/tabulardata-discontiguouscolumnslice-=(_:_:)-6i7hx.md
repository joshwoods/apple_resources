

- TabularData
- DiscontiguousColumnSlice
-  /=(\_:\_:) 

Operator

# /=(\_:\_:)

Modifies a floating-point column slice by dividing each element by a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func /= (lhs: inout DiscontiguousColumnSlice, rhs: WrappedElement) where WrappedElement : FloatingPoint
```

## Parameters 

`lhs`  

A column slice.

`rhs`  

A value of the same type as the column’s elements.

## See Also

### Modifying a Column Slice with a Value

static func += (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies a column slice by adding a value to each element.

static func -= (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies a column slice by subtracting a value from each element.

static func *= (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies a column slice by multiplying each element by a value.

static func /= (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies an integer column slice by dividing each element by a value.

