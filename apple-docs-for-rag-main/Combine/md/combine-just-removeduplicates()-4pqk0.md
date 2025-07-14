

- Combine
- Just
-  removeDuplicates() 

Instance Method

# removeDuplicates()

Publishes only elements that don’t match the previous element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func removeDuplicates() -> Publishers.RemoveDuplicates
```

Available when `Output` conforms to `Equatable`.

## Return Value

A publisher that consumes — rather than publishes — duplicate elements.

## Discussion

Use removeDuplicates() to remove repeating elements from an upstream publisher. This operator has a two-element memory: the operator uses the current and previously published elements as the basis for its comparison.

In the example below, removeDuplicates() triggers on the doubled, tripled, and quadrupled occurrences of `1`, `3`, and `4` respectively. Because the two-element memory considers only the current element and the previous element, the operator prints the final `0` in the example data since its immediate predecessor is `4`.

```
let numbers = [0, 1, 2, 2, 3, 3, 3, 4, 4, 4, 4, 0]
cancellable = numbers.publisher
    .removeDuplicates()
    .sink { print("\($0)", terminator: " ") }

// Prints: "0 1 2 3 4 0"
```

