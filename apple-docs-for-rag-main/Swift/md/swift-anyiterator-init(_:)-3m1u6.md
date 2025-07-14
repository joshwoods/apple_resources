

- Swift
- AnyIterator
-  init(\_:) 

Initializer

# init(\_:)

Creates an iterator that wraps a base iterator but whose type depends only on the base iterator’s element type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ base: I) where Element == I.Element, I : IteratorProtocol
```

## Parameters 

`base`  

An iterator to type-erase.

## Discussion

You can use `AnyIterator` to hide the type signature of a more complex iterator. For example, the `digits()` function in the following example creates an iterator over a collection that lazily maps the elements of a `Range` instance to strings. Instead of returning an iterator with a type that encapsulates the implementation of the collection, the `digits()` function first wraps the iterator in an `AnyIterator` instance.

```
func digits() -> AnyIterator {
    let lazyStrings = (0.., String>.Iterator
        = lazyStrings.makeIterator()

    return AnyIterator(iterator)
}
```

