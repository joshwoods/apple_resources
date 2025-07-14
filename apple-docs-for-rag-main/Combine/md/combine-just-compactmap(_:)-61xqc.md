

- Combine
- Just
-  compactMap(\_:) 

Instance Method

# compactMap(\_:)

Calls a closure with each received element and publishes any returned optional that has a value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func compactMap(_ transform: @escaping (Self.Output) -> T?) -> Publishers.CompactMap
```

## Parameters 

`transform`  

A closure that receives a value and returns an optional value.

## Return Value

Any non-`nil` optional results of the calling the supplied closure.

## Discussion

Combine’s compactMap(_:) operator performs a function similar to that of compactMap(_:) in the Swift standard library: the compactMap(_:) operator in Combine removes `nil` elements in a publisher’s stream and republishes non-`nil` elements to the downstream subscriber.

The example below uses a range of numbers as the source for a collection based publisher. The compactMap(_:) operator consumes each element from the `numbers` publisher attempting to access the dictionary using the element as the key. If the example’s dictionary returns a `nil`, due to a non-existent key, compactMap(_:) filters out the `nil` (missing) elements.

```
let numbers = (0...5)
let romanNumeralDict: [Int : String] =
    [1: "I", 2: "II", 3: "III", 5: "V"]

cancellable = numbers.publisher
    .compactMap { romanNumeralDict[$0] }
    .sink { print("\($0)", terminator: " ") }

// Prints: "I II III V"
```

