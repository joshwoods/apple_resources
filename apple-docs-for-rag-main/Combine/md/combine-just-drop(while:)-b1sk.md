

- Combine
- Just
-  drop(while:) 

Instance Method

# drop(while:)

Omits elements from the upstream publisher until a given closure returns false, before republishing all remaining elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func drop(while predicate: @escaping (Self.Output) -> Bool) -> Publishers.DropWhile
```

## Parameters 

`predicate`  

A closure that takes an element as a parameter and returns a Boolean value indicating whether to drop the element from the publisher’s output.

## Return Value

A publisher that skips over elements until the provided closure returns `false`.

## Discussion

Use drop(while:) to omit elements from an upstream publisher until the element received meets a condition you specify.

In the example below, the operator omits all elements in the stream until the first element arrives that’s a positive integer, after which the operator publishes all remaining elements:

```
let numbers = [-62, -1, 0, 10, 0, 22, 41, -1, 5]
cancellable = numbers.publisher
    .drop { $0 

