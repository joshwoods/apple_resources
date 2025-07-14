

- Combine
- Publishers
- Publishers.Breakpoint
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

## See Also

### Filtering Elements

func filter((Self.Output) -> Bool) -> Publishers.Filter&lt;Self>

Republishes all elements that match a provided closure.

func tryFilter((Self.Output) throws -> Bool) -> Publishers.TryFilter&lt;Self>

Republishes all elements that match a provided error-throwing closure.

func tryCompactMap&lt;T>((Self.Output) throws -> T?) -> Publishers.TryCompactMap&lt;Self, T>

Calls an error-throwing closure with each received element and publishes any returned optional that has a value.

func removeDuplicates() -> Publishers.RemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element.

func removeDuplicates(by: (Self.Output, Self.Output) -> Bool) -> Publishers.RemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element, as evaluated by a provided closure.

func tryRemoveDuplicates(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryRemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

func replaceEmpty(with: Self.Output) -> Publishers.ReplaceEmpty&lt;Self>

Replaces an empty stream with the provided element.

func replaceError(with: Self.Output) -> Publishers.ReplaceError&lt;Self>

Replaces any errors in the stream with the provided element.

