

- RealityKit
- Scene
- Scene.Publisher
-  tryPrefix(while:) 

Instance Method

# tryPrefix(while:)

Republishes elements while an error-throwing predicate closure indicates publishing should continue.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

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

## See Also

### Applying sequence operations to elements

func drop&lt;P>(untilOutputFrom: P) -> Publishers.DropUntilOutput&lt;Self, P>

Ignores elements from the upstream publisher until it receives an element from a second publisher.

func drop(while: (Self.Output) -> Bool) -> Publishers.DropWhile&lt;Self>

Omits elements from the upstream publisher until a given closure returns false, before republishing all remaining elements.

func dropFirst(Int) -> Publishers.Drop&lt;Self>

Omits the specified number of elements before republishing subsequent elements.

func tryDrop(while: (Self.Output) throws -> Bool) -> Publishers.TryDropWhile&lt;Self>

Omits elements from the upstream publisher until an error-throwing closure returns false, before republishing all remaining elements.

func append(Self.Output...) -> Publishers.Concatenate&lt;Self, Publishers.Sequence&lt;[Self.Output], Self.Failure>>

Appends a publisher’s output with the specified elements.

func prepend(Self.Output...) -> Publishers.Concatenate&lt;Publishers.Sequence&lt;[Self.Output], Self.Failure>, Self>

Prefixes a publisher’s output with the specified values.

func prefix(Int) -> Publishers.Output&lt;Self>

Republishes elements up to the specified maximum count.

func prefix&lt;P>(untilOutputFrom: P) -> Publishers.PrefixUntilOutput&lt;Self, P>

Republishes elements until another publisher emits an element.

func prefix(while: (Self.Output) -> Bool) -> Publishers.PrefixWhile&lt;Self>

Republishes elements while a predicate closure indicates publishing should continue.

