

- Combine
- Deferred
-  tryContains(where:) 

Instance Method

# tryContains(where:)

Publishes a Boolean value upon receiving an element that satisfies the throwing predicate closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryContains(where predicate: @escaping (Self.Output) throws -> Bool) -> Publishers.TryContainsWhere
```

## Parameters 

`predicate`  

A closure that takes an element as its parameter and returns a Boolean value that indicates whether the element satisfies the closure’s comparison logic.

## Return Value

A publisher that emits the Boolean value `true` when the upstream publisher emits a matching value.

## Discussion

Use tryContains(where:) to find the first element in an upstream that satisfies the error-throwing closure you provide.

This operator consumes elements produced from the upstream publisher until the upstream publisher either:

- Produces a matching element, after which it emits `true` and the publisher finishes normally.

- Emits `false` if no matching element is found and the publisher finishes normally.

If the predicate throws an error, the publisher fails, passing the error to its downstream.

In the example below, the tryContains(where:) operator tests values to find an element less than `10`; when the closure finds an odd number, like `3`, the publisher terminates with an `IllegalValueError`.

```
struct IllegalValueError: Error {}

let numbers = [3, 2, 10, 5, 0, 9]
numbers.publisher
    .tryContains {
        if ($0 % 2 != 0) {
            throw IllegalValueError()
        }
       return $0 

## See Also

### Applying Matching Criteria to Elements

func contains(Self.Output) -> Publishers.Contains&lt;Self>

Publishes a Boolean value upon receiving an element equal to the argument.

func contains(where: (Self.Output) -> Bool) -> Publishers.ContainsWhere&lt;Self>

Publishes a Boolean value upon receiving an element that satisfies the predicate closure.

func allSatisfy((Self.Output) -> Bool) -> Publishers.AllSatisfy&lt;Self>

Publishes a single Boolean value that indicates whether all received elements pass a given predicate.

func tryAllSatisfy((Self.Output) throws -> Bool) -> Publishers.TryAllSatisfy&lt;Self>

Publishes a single Boolean value that indicates whether all received elements pass a given error-throwing predicate.

