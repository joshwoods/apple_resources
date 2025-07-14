

- Core ML
-  MLShapedArrayRangeExpression 

Protocol

# MLShapedArrayRangeExpression

An interface for a range expression, which you typically use with subscripts of shaped array types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol MLShapedArrayRangeExpression
```

## Topics

### Generating Relative Ranges

func relative(toShapedArrayAxis: Range&lt;Int>) -> Range&lt;Int>

Returns the range of indices the range expression describes within a collection.

**Required**

## See Also

### Supporting Types

associatedtype Scalar : MLShapedArrayScalar

Represents the underlying scalar type of the shaped array type.

**Required**

struct MLShapedArraySlice

A multidimensional subset of elements from a shaped array type.

protocol MLShapedArrayScalar

A type that associates a scalar with a shaped array.

