

- Combine
- CurrentValueSubject
-  scan(\_:\_:) 

Instance Method

# scan(\_:\_:)

Transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func scan(
    _ initialResult: T,
    _ nextPartialResult: @escaping (T, Self.Output) -> T
) -> Publishers.Scan
```

## Parameters 

`initialResult`  

The previous result returned by the `nextPartialResult` closure.

`nextPartialResult`  

A closure that takes as its arguments the previous value returned by the closure and the next element emitted from the upstream publisher.

## Return Value

A publisher that transforms elements by applying a closure that receives its previous return value and the next element from the upstream publisher.

## Discussion

Use scan(_:_:) to accumulate all previously-published values into a single value, which you then combine with each newly-published value.

The following example logs a running total of all values received from the sequence publisher.

```
let range = (0...5)
cancellable = range.publisher
    .scan(0) { return $0 + $1 }
    .sink { print ("\($0)", terminator: " ") }
 // Prints: "0 1 3 6 10 15 ".
```

## See Also

### Mapping Elements

func map&lt;T>((Self.Output) -> T) -> Publishers.Map&lt;Self, T>

Transforms all elements from the upstream publisher with a provided closure.

func tryMap&lt;T>((Self.Output) throws -> T) -> Publishers.TryMap&lt;Self, T>

Transforms all elements from the upstream publisher with a provided error-throwing closure.

func mapError&lt;E>((Self.Failure) -> E) -> Publishers.MapError&lt;Self, E>

Converts any failure from the upstream publisher into a new error.

func replaceNil&lt;T>(with: T) -> Publishers.Map&lt;Self, T>

Replaces nil elements in the stream with the provided element.

func tryScan&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryScan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to an error-throwing closure along with the last value returned by the closure.

func setFailureType&lt;E>(to: E.Type) -> Publishers.SetFailureType&lt;Self, E>

Changes the failure type declared by the upstream publisher.

