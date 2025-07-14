

- Swift
- AnyIterator
-  init(\_:) 

Initializer

# init(\_:)

Creates an iterator that wraps the given closure in its `next()` method.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ body: @escaping () -> Element?)
```

## Parameters 

`body`  

A closure that returns an optional element. `body` is executed each time the `next()` method is called on the resulting iterator.

## Discussion

The following example creates an iterator that counts up from the initial value of an integer `x` to 15:

```
var x = 7
let iterator: AnyIterator = AnyIterator {
    defer { x += 1 }
    return x 

