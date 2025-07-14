

- Combine
- Just
-  prefix(while:) 

Instance Method

# prefix(while:)

Republishes elements while a predicate closure indicates publishing should continue.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func prefix(while predicate: @escaping (Self.Output) -> Bool) -> Publishers.PrefixWhile
```

## Parameters 

`predicate`  

A closure that takes an element as its parameter and returns a Boolean value that indicates whether publishing should continue.

## Return Value

A publisher that passes through elements until the predicate indicates publishing should finish.

## Discussion

Use prefix(while:) to emit values while elements from the upstream publisher meet a condition you specify. The publisher finishes when the closure returns `false`.

In the example below, the prefix(while:) operator emits values while the element it receives is less than five:

```
let numbers = (0...10)
numbers.publisher
    .prefix { $0 

