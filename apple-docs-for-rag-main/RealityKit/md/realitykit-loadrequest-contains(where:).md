

- RealityKit
- LoadRequest
-  contains(where:) 

Instance Method

# contains(where:)

Publishes a Boolean value upon receiving an element that satisfies the predicate closure.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func contains(where predicate: @escaping (Self.Output) -> Bool) -> Publishers.ContainsWhere
```

## Parameters 

`predicate`  

A closure that takes an element as its parameter and returns a Boolean value that indicates whether the element satisfies the closure’s comparison logic.

## Return Value

A publisher that emits the Boolean value `true` when the upstream publisher emits a matching value.

## Discussion

Use `Publisher/contains(where:)` to find the first element in an upstream that satisfies the closure you provide. This operator consumes elements produced from the upstream publisher until the upstream publisher produces a matching element.

This operator is useful when the upstream publisher produces elements that don’t conform to `Equatable`.

In the example below, the `Publisher/contains(where:)` operator tests elements against the supplied closure and emits `true` for the first elements that’s greater than `4`, and then finishes normally.

```
let numbers = [-1, 0, 10, 5]
numbers.publisher
    .contains {$0 > 4}
    .sink { print("\($0)") }

// Prints: "true"
```

## See Also

### Applying matching criteria to elements

func contains(Self.Output) -> Publishers.Contains&lt;Self>

Publishes a Boolean value upon receiving an element equal to the argument.

func tryContains(where: (Self.Output) throws -> Bool) -> Publishers.TryContainsWhere&lt;Self>

Publishes a Boolean value upon receiving an element that satisfies the throwing predicate closure.

func allSatisfy((Self.Output) -> Bool) -> Publishers.AllSatisfy&lt;Self>

Publishes a single Boolean value that indicates whether all received elements pass a given predicate.

func tryAllSatisfy((Self.Output) throws -> Bool) -> Publishers.TryAllSatisfy&lt;Self>

Publishes a single Boolean value that indicates whether all received elements pass a given error-throwing predicate.

