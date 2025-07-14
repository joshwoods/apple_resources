

- Swift
- String
- String.UnicodeScalarView
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Appends the Unicode scalar values in the given sequence to the view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func append(contentsOf newElements: S) where S : Sequence, S.Element == Unicode.Scalar
```

## Parameters 

`newElements`  

A sequence of Unicode scalar values.

## Discussion

Complexity

O(*n*), where *n* is the length of the resulting view.

