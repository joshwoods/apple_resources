

- Combine
- Just
-  last(where:) 

Instance Method

# last(where:)

Publishes the last element of a stream that satisfies a predicate closure, after upstream finishes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func last(where predicate: @escaping (Self.Output) -> Bool) -> Publishers.LastWhere
```

## Parameters 

`predicate`  

A closure that takes an element as its parameter and returns a Boolean value that indicates whether to publish the element.

## Return Value

A publisher that only publishes the last element satisfying the given predicate.

## Discussion

Use last(where:) when you need to republish only the last element of a stream that satisfies a closure you specify.

In the example below, a range publisher emits the last element that satisfies the closure’s criteria, then finishes normally:

```
let numbers = (-10...10)
cancellable = numbers.publisher
    .last { $0 

