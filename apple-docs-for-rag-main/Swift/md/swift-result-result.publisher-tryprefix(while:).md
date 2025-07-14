

- Swift
- Result
- Result.Publisher
-  tryPrefix(while:) 

Instance Method

# tryPrefix(while:)

Republishes elements while an error-throwing predicate closure indicates publishing should continue.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryPrefix(while predicate: @escaping (Self.Output) throws -> Bool) -> Publishers.TryPrefixWhile
```

## Parameters 

`predicate`  

A closure that takes an element as its parameter and returns a Boolean value indicating whether publishing should continue.

## Return Value

A publisher that passes through elements until the predicate throws or indicates publishing should finish.

## Discussion

Use tryPrefix(while:) to emit values from the upstream publisher that meet a condition you specify in an error-throwing closure. The publisher finishes when the closure returns `false`. If the closure throws an error, the publisher fails with that error.

```
struct OutOfRangeError: Error {}

let numbers = (0...10).reversed()
cancellable = numbers.publisher
    .tryPrefix {
        guard $0 != 0 else {throw OutOfRangeError()}
        return $0 

