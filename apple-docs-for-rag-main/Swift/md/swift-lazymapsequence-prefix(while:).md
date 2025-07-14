

- Swift
- LazyMapSequence
-  prefix(while:) 

Instance Method

# prefix(while:)

Returns a lazy sequence of the initial consecutive elements that satisfy `predicate`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func prefix(while predicate: @escaping (Self.Elements.Element) -> Bool) -> LazyPrefixWhileSequence
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns `true` if the element should be included or `false` otherwise. Once `predicate` returns `false` it will not be called again.

