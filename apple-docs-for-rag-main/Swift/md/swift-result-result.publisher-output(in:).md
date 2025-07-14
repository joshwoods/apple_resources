

- Swift
- Result
- Result.Publisher
-  output(in:) 

Instance Method

# output(in:)

Publishes elements specified by their range in the sequence of published elements.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func output(in range: R) -> Publishers.Output where R : RangeExpression, R.Bound == Int
```

## Parameters 

`range`  

A range that indicates which elements to publish.

## Return Value

A publisher that publishes elements specified by a range.

## Discussion

Use output(in:) to republish a range indices you specify in the published stream. After publishing all elements, the publisher finishes normally. If the publisher completes normally or with an error before producing all the elements in the range, it doesn’t publish the remaining elements.

In the example below, an array publisher emits the subset of elements at the indices in the specified range:

```
let numbers = [1, 1, 2, 2, 2, 3, 4, 5, 6]
numbers.publisher
    .output(in: (3...5))
    .sink { print("\($0)", terminator: " ") }

// Prints: "2 2 3"
```

