

- Swift
- SIMDMask
-  init(\_:) 

Initializer

# init(\_:)

Creates a vector from the given sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ scalars: S) where S : Sequence, Self.Scalar == S.Element
```

## Parameters 

`scalars`  

The elements to use in the vector.

## Discussion

Precondition

`scalars` must have the same number of elements as the vector type.

