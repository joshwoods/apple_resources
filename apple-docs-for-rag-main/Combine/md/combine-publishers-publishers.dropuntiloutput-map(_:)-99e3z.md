

- Combine
- Publishers
- Publishers.DropUntilOutput
-  map(\_:) 

Instance Method

# map(\_:)

Transforms all elements from the upstream publisher with a provided closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func map(_ transform: @escaping (Self.Output) -> T) -> Publishers.Map
```

## Parameters 

`transform`  

A closure that takes one element as its parameter and returns a new element.

## Return Value

A publisher that uses the provided closure to map elements from the upstream publisher to new elements that it then publishes.

## Discussion

Combine’s map(_:) operator performs a function similar to that of map(_:) in the Swift standard library: it uses a closure to transform each element it receives from the upstream publisher. You use map(_:) to transform from one kind of element to another.

The following example uses an array of numbers as the source for a collection based publisher. A map(_:) operator consumes each integer from the publisher and uses a dictionary to transform it from its Arabic numeral to a Roman equivalent, as a String. If the map(_:)’s closure fails to look up a Roman numeral, it returns the string `(unknown)`.

```
let numbers = [5, 4, 3, 2, 1, 0]
let romanNumeralDict: [Int : String] =
   [1:"I", 2:"II", 3:"III", 4:"IV", 5:"V"]
cancellable = numbers.publisher
    .map { romanNumeralDict[$0] ?? "(unknown)" }
    .sink { print("\($0)", terminator: " ") }

// Prints: "V IV III II I (unknown)"
```

If your closure can throw an error, use Combine’s tryMap(_:) operator instead.

## See Also

### Mapping Elements

func tryMap&lt;T>((Self.Output) throws -> T) -> Publishers.TryMap&lt;Self, T>

Transforms all elements from the upstream publisher with a provided error-throwing closure.

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

