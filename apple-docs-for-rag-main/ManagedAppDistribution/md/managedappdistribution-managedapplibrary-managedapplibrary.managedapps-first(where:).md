

- ManagedAppDistribution
- ManagedAppLibrary
- ManagedAppLibrary.ManagedApps
-  first(where:) 

Instance Method

# first(where:)

Returns the first element of the sequence that satisfies the given predicate.

ManagedAppDistributionSwiftiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func first(where predicate: (Self.Element) async throws -> Bool) async rethrows -> Self.Element?
```

## Parameters 

`predicate`  

A closure that takes an element of the asynchronous sequence as its argument and returns a Boolean value that indicates whether the element is a match.

## Return Value

The first element of the sequence that satisfies `predicate`, or `nil` if there is no element that satisfies `predicate`.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `first(where:)` method returns the first member of the sequence that’s evenly divisible by both `2` and `3`.

```
let divisibleBy2And3 = await Counter(howHigh: 10)
    .first { $0 % 2 == 0 && $0 % 3 == 0 }
print(divisibleBy2And3 ?? "none")
// Prints "6"
```

The predicate executes each time the asynchronous sequence produces an element, until either the predicate finds a match or the sequence ends.

