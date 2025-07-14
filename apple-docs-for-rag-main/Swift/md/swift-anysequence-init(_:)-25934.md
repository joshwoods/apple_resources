

- Swift
- AnySequence
-  init(\_:) 

Initializer

# init(\_:)

Creates a sequence whose `makeIterator()` method forwards to `makeUnderlyingIterator`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ makeUnderlyingIterator: @escaping () -> I) where Element == I.Element, I : IteratorProtocol
```

