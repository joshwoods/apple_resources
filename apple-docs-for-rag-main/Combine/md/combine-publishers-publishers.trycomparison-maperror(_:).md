

- Combine
- Publishers
- Publishers.TryComparison
-  mapError(\_:) 

Instance Method

# mapError(\_:)

Converts any failure from the upstream publisher into a new error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func mapError(_ transform: @escaping (Self.Failure) -> E) -> Publishers.MapError where E : Error
```

## Parameters 

`transform`  

A closure that takes the upstream failure as a parameter and returns a new error for the publisher to terminate with.

## Return Value

A publisher that replaces any upstream failure with a new error produced by the `transform` closure.

## Discussion

Use the mapError(_:) operator when you need to replace one error type with another, or where a downstream operator needs the error types of its inputs to match.

The following example uses a tryMap(_:) operator to divide `1` by each element produced by a sequence publisher. When the publisher produces a `0`, the tryMap(_:) fails with a `DivisionByZeroError`. The mapError(_:) operator converts this into a `MyGenericError`.

```
struct DivisionByZeroError: Error {}
struct MyGenericError: Error { var wrappedError: Error }

func myDivide(_ dividend: Double, _ divisor: Double) throws -> Double {
       guard divisor != 0 else { throw DivisionByZeroError() }
       return dividend / divisor
   }

let divisors: [Double] = [5, 4, 3, 2, 1, 0]
divisors.publisher
    .tryMap { try myDivide(1, $0) }
    .mapError { MyGenericError(wrappedError: $0) }
    .sink(
        receiveCompletion: { print ("completion: \($0)") ,
        receiveValue: { print ("value: \($0)", terminator: " ") }
     )

// Prints: "0.2 0.25 0.3333333333333333 0.5 1.0 completion: failure(MyGenericError(wrappedError: DivisionByZeroError()))"
```

## See Also

### Mapping Elements

func map&lt;T>((Self.Output) -> T) -> Publishers.Map&lt;Self, T>

Transforms all elements from the upstream publisher with a provided closure.

func tryMap&lt;T>((Self.Output) throws -> T) -> Publishers.TryMap&lt;Self, T>

Transforms all elements from the upstream publisher with a provided error-throwing closure.

func replaceNil&lt;T>(with: T) -> Publishers.Map&lt;Self, T>

Replaces nil elements in the stream with the provided element.

func scan&lt;T>(T, (T, Self.Output) -> T) -> Publishers.Scan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

func tryScan&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryScan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to an error-throwing closure along with the last value returned by the closure.

