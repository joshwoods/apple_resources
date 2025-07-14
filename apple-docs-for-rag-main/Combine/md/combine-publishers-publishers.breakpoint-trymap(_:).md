

- Combine
- Publishers
- Publishers.Breakpoint
-  tryMap(\_:) 

Instance Method

# tryMap(\_:)

Transforms all elements from the upstream publisher with a provided error-throwing closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryMap(_ transform: @escaping (Self.Output) throws -> T) -> Publishers.TryMap
```

## Parameters 

`transform`  

A closure that takes one element as its parameter and returns a new element. If the closure throws an error, the publisher fails with the thrown error.

## Return Value

A publisher that uses the provided closure to map elements from the upstream publisher to new elements that it then publishes.

## Discussion

Combine’s tryMap(_:) operator performs a function similar to that of map(_:) in the Swift standard library: it uses a closure to transform each element it receives from the upstream publisher. You use tryMap(_:) to transform from one kind of element to another, and to terminate publishing when the map’s closure throws an error.

The following example uses an array of numbers as the source for a collection based publisher. A tryMap(_:) operator consumes each integer from the publisher and uses a dictionary to transform it from its Arabic numeral to a Roman equivalent, as a String. If the tryMap(_:)’s closure fails to look up a Roman numeral, it throws an error. The tryMap(_:) operator catches this error and terminates publishing, sending a Subscribers.Completion.failure(_:) that wraps the error.

```
struct ParseError: Error {}
func romanNumeral(from:Int) throws -> String {
    let romanNumeralDict: [Int : String] =
        [1:"I", 2:"II", 3:"III", 4:"IV", 5:"V"]
    guard let numeral = romanNumeralDict[from] else {
        throw ParseError()
    }
    return numeral
}
let numbers = [5, 4, 3, 2, 1, 0]
cancellable = numbers.publisher
    .tryMap { try romanNumeral(from: $0) }
    .sink(
        receiveCompletion: { print ("completion: \($0)") },
        receiveValue: { print ("\($0)", terminator: " ") }
     )

// Prints: "V IV III II I completion: failure(ParseError())"
```

If your closure doesn’t throw, use map(_:) instead.

## See Also

### Mapping Elements

func map&lt;T>((Self.Output) -> T) -> Publishers.Map&lt;Self, T>

Transforms all elements from the upstream publisher with a provided closure.

func mapError&lt;E>((Self.Failure) -> E) -> Publishers.MapError&lt;Self, E>

Converts any failure from the upstream publisher into a new error.

func replaceNil&lt;T>(with: T) -> Publishers.Map&lt;Self, T>

Replaces nil elements in the stream with the provided element.

func scan&lt;T>(T, (T, Self.Output) -> T) -> Publishers.Scan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

func tryScan&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryScan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to an error-throwing closure along with the last value returned by the closure.

func setFailureType&lt;E>(to: E.Type) -> Publishers.SetFailureType&lt;Self, E>

Changes the failure type declared by the upstream publisher.

