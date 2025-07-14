

- Swift
- LazyMapSequence
-  drop(while:) 

Instance Method

# drop(while:)

Returns a lazy sequence that skips any initial elements that satisfy `predicate`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func drop(while predicate: @escaping (Self.Elements.Element) -> Bool) -> LazyDropWhileSequence
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns `true` if the element should be skipped or `false` otherwise. Once `predicate` returns `false` it will not be called again.

