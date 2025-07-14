

- Swift
- LazyMapSequence
-  compactMap(\_:) 

Instance Method

# compactMap(\_:)

Returns the non-`nil` results of mapping the given transformation over this sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compactMap(_ transform: @escaping (Self.Elements.Element) -> ElementOfResult?) -> LazyMapSequence>, ElementOfResult>
```

## Parameters 

`transform`  

A closure that accepts an element of this sequence as its argument and returns an optional value.

## Discussion

Use this method to receive a sequence of non-optional values when your transformation produces an optional value.

Complexity

O(1)

