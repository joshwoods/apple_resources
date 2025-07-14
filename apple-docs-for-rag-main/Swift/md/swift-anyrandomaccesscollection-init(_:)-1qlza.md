

- Swift
- AnyRandomAccessCollection
-  init(\_:) 

Initializer

# init(\_:)

Creates a type-erased collection that wraps the given collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ base: C) where Element == C.Element, C : RandomAccessCollection
```

## Parameters 

`base`  

The collection to wrap.

## Discussion

Complexity

O(1).

