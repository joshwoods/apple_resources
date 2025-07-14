

- Create ML Components
- MLModelClassifierAdaptor
- MLModelClassifierAdaptor.Label
-  MLModelClassifierAdaptor.Label.IntegerLiteralType 

Type Alias

# MLModelClassifierAdaptor.Label.IntegerLiteralType

A type that represents an integer literal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias IntegerLiteralType = Int
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Discussion

The standard library integer and floating-point types are all valid types for `IntegerLiteralType`.

