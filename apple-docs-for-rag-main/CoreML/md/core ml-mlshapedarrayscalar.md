

- Core ML
-  MLShapedArrayScalar 

Protocol

# MLShapedArrayScalar

A type that associates a scalar with a shaped array.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol MLShapedArrayScalar
```

## Topics

### Determining the Underlying Type

static var multiArrayDataType: MLMultiArrayDataType

The shaped array’s scalar type as a multiarray data type.

**Required**

## See Also

### Supporting Types

associatedtype Scalar : MLShapedArrayScalar

Represents the underlying scalar type of the shaped array type.

**Required**

struct MLShapedArraySlice

A multidimensional subset of elements from a shaped array type.

protocol MLShapedArrayRangeExpression

An interface for a range expression, which you typically use with subscripts of shaped array types.

