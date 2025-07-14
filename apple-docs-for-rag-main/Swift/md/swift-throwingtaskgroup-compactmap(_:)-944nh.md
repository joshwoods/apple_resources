

- Swift
- ThrowingTaskGroup
-  compactMap(\_:) 

Instance Method

# compactMap(\_:)

Creates an asynchronous sequence that maps an error-throwing closure over the base sequence’s elements, omitting results that don’t return a value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
func compactMap(_ transform: @escaping (Self.Element) async throws -> ElementOfResult?) -> AsyncThrowingCompactMapSequence
```

## Parameters 

`transform`  

An error-throwing mapping closure. `transform` accepts an element of this sequence as its parameter and returns a transformed value of the same or of a different type. If `transform` throws an error, the sequence ends.

## Return Value

An asynchronous sequence that contains, in order, the non-`nil` elements produced by the `transform` closure. The sequence ends either when the base sequence ends or when `transform` throws an error.

## Discussion

Use the `compactMap(_:)` method to transform every element received from a base asynchronous sequence, while also discarding any `nil` results from the closure. Typically, you use this to transform from one type of element to another.

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `5`. The closure provided to the `compactMap(_:)` method takes each `Int` and looks up a corresponding `String` from a `romanNumeralDict` dictionary. Since there is no key for `4`, the closure returns `nil` in this case, which `compactMap(_:)` omits from the transformed asynchronous sequence. When the value is `5`, the closure throws `MyError`, terminating the sequence.

```
let romanNumeralDict: [Int: String] =
    [1: "I", 2: "II", 3: "III", 5: "V"]

do {
    let stream = Counter(howHigh: 5)
        .compactMap { (value) throws -> String? in
            if value == 5 {
                throw MyError()
            }
            return romanNumeralDict[value]
        }
    for try await numeral in stream {
        print(numeral, terminator: " ")
    }
} catch {
    print("Error: \(error)")
}
// Prints "I II III Error: MyError() "
```

## See Also

### Accessing an Asynchronous Sequence of Results

func makeAsyncIterator() -> ThrowingTaskGroup&lt;ChildTaskResult, Failure>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

func allSatisfy((Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether all elements produced by the asynchronous sequence satisfy the given predicate.

func compactMap&lt;ElementOfResult>((Self.Element) async -> ElementOfResult?) -> AsyncCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements, omitting results that don’t return a value.

func contains(Self.Element) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains the given element.

func contains(where: (Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains an element that satisfies the given predicate.

func drop(while: (Self.Element) async -> Bool) -> AsyncDropWhileSequence&lt;Self>

Omits elements from the base asynchronous sequence until a given closure returns false, after which it passes through all remaining elements.

func dropFirst(Int) -> AsyncDropFirstSequence&lt;Self>

Omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

func filter((Self.Element) async -> Bool) -> AsyncFilterSequence&lt;Self>

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate.

func first(where: (Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func map&lt;Transformed>((Self.Element) async throws -> Transformed) -> AsyncThrowingMapSequence&lt;Self, Transformed>

Creates an asynchronous sequence that maps the given error-throwing closure over the asynchronous sequence’s elements.

func map&lt;Transformed>((Self.Element) async -> Transformed) -> AsyncMapSequence&lt;Self, Transformed>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements.

func max() async rethrows -> Self.Element?

Returns the maximum element in an asynchronous sequence of comparable elements.

func max(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the maximum element in the asynchronous sequence, using the given predicate as the comparison between elements.

func min() async rethrows -> Self.Element?

Returns the minimum element in an asynchronous sequence of comparable elements.

func min(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the minimum element in the asynchronous sequence, using the given predicate as the comparison between elements.

