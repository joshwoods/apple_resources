

- ActivityKit
- Activity
- Activity.ContentStateUpdates
-  min() 

Instance Method

# min()

Returns the minimum element in an asynchronous sequence of comparable elements.

ActivityKitSwiftiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
@warn_unqualified_access
func min() async rethrows -> Self.Element?
```

Available when `Element` conforms to `Comparable`.

## Return Value

The sequence’s minimum element. If the sequence has no elements, returns `nil`.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `min()` method returns the minimum value of the sequence.

```
let min = await Counter(howHigh: 10)
    .min()
print(min ?? "none")
// Prints "1"
```

