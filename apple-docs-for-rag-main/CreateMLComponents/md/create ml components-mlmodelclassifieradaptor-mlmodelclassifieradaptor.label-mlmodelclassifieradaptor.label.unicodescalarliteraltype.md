

- Create ML Components
- MLModelClassifierAdaptor
- MLModelClassifierAdaptor.Label
-  MLModelClassifierAdaptor.Label.UnicodeScalarLiteralType 

Type Alias

# MLModelClassifierAdaptor.Label.UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias UnicodeScalarLiteralType = String
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Discussion

Valid types for `UnicodeScalarLiteralType` are `Unicode.Scalar`, `Character`, `String`, and `StaticString`.

