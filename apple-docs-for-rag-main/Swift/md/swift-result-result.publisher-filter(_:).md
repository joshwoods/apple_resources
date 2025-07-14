

- Swift
- Result
- Result.Publisher
-  filter(\_:) 

Instance Method

# filter(\_:)

Republishes all elements that match a provided closure.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func filter(_ isIncluded: @escaping (Self.Output) -> Bool) -> Publishers.Filter
```

## Parameters 

`isIncluded`  

A closure that takes one element and returns a Boolean value indicating whether to republish the element.

## Return Value

A publisher that republishes all elements that satisfy the closure.

## Discussion

Combine’s filter(_:) operator performs an operation similar to that of filter(_:) in the Swift Standard Library: it uses a closure to test each element to determine whether to republish the element to the downstream subscriber.

The following example, uses a filter operation that receives an `Int` and only republishes a value if it’s even.

```
let numbers: [Int] = [1, 2, 3, 4, 5]
cancellable = numbers.publisher
    .filter { $0 % 2 == 0 }
    .sink { print("\($0)", terminator: " ") }

// Prints: "2 4"
```

