

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.Updates
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the asynchronous sequence contains the given element.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
func contains(_ search: Self.Element) async rethrows -> Bool
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`search`  

The element to find in the asynchronous sequence.

## Return Value

`true` if the method found the element in the asynchronous sequence; otherwise, `false`.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `contains(_:)` method checks to see whether the sequence produces the value `5`:

```
let containsFive = await Counter(howHigh: 10)
    .contains(5)
print(containsFive)
// Prints "true"
```

