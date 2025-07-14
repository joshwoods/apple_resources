

- Create ML Components
- ComposedTransformer
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
static func == (a: ComposedTransformer, b: ComposedTransformer) -> Bool
```

Available when `Inner` conforms to `Transformer`, `Inner` conforms to `Equatable`, `Outer` conforms to `Transformer`, `Outer` conforms to `Equatable`, and `Inner.Output` is `Outer.Input`.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

