

- Swift
- AsyncThrowingDropWhileSequence
-  max() 

Instance Method

# max()

Returns the maximum element in an asynchronous sequence of comparable elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@warn_unqualified_access
func max() async rethrows -> Self.Element?
```

Available when `Element` conforms to `Comparable`.

## Return Value

The sequence’s maximum element. If the sequence has no elements, returns `nil`.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `max()` method returns the max value of the sequence.

```
let max = await Counter(howHigh: 10)
    .max()
print(max ?? "none")
// Prints "10"
```

