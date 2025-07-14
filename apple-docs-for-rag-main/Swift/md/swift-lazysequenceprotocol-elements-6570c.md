

- Swift
- LazySequenceProtocol
-  elements 

Instance Property

# elements

A sequence containing the same elements as this one, possibly with a simpler type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var elements: Self.Elements { get }
```

**Required** Default implementation provided.

## Discussion

When implementing lazy operations, wrapping `elements` instead of `self` can prevent result types from growing an extra `LazySequence` layer.

Note: this property need not be implemented by conforming types, it has a default implementation in a protocol extension that just returns `self`.

## Default Implementations

### LazySequenceProtocol Implementations

var elements: Self

Identical to `self`.

