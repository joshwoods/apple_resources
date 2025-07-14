

- Swift
- Result
- Result.Publisher
-  dropFirst(\_:) 

Instance Method

# dropFirst(\_:)

Omits the specified number of elements before republishing subsequent elements.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func dropFirst(_ count: Int = 1) -> Publishers.Drop
```

## Parameters 

`count`  

The number of elements to omit. The default is `1`.

## Return Value

A publisher that doesn’t republish the first `count` elements.

## Discussion

Use dropFirst(_:) when you want to drop the first `n` elements from the upstream publisher, and republish the remaining elements.

The example below drops the first five elements from the stream:

```
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
cancellable = numbers.publisher
    .dropFirst(5)
    .sink { print("\($0)", terminator: " ") }

// Prints: "6 7 8 9 10 "
```

