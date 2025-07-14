

- Combine
-  Future 

Class

# Future

A publisher that eventually produces a single value and then finishes or fails.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class Future where Failure : Error
```

## Mentioned in 

Using Combine for Your App’s Asynchronous Code

## Overview

Use a future to perform some work and then asynchronously publish a single element. You initialize the future with a closure that takes a Future.Promise; the closure calls the promise with a Result that indicates either success or failure. In the success case, the future’s downstream subscriber receives the element prior to the publishing stream finishing normally. If the result is an error, publishing terminates with that error.

The following example shows a method that uses a future to asynchronously publish a random number after a brief delay:

```
func generateAsyncRandomNumberFromFuture() -> Future  {
    return Future() { promise in
        DispatchQueue.main.asyncAfter(deadline: .now() + 2) {
            let number = Int.random(in: 1...10)
            promise(Result.success(number))
        }
    }
}
```

To receive the published value, you use any Combine subscriber, such as a Subscribers.Sink, like this:

```
cancellable = generateAsyncRandomNumberFromFuture()
    .sink { number in print("Got random number \(number).") }
```

### Integrating with Swift Concurrency

To integrate with the `async`-`await` syntax in Swift 5.5, `Future` can provide its value to an awaiting caller. This is particularly useful because unlike other types that conform to Publisher and potentially publish many elements, a `Future` only publishes one element (or fails). By using the value property, the above call point looks like this:

```
let number = await generateAsyncRandomNumberFromFuture().value
print("Got random number \(number).")
```

### Alternatives to Futures

The `async`-`await` syntax in Swift can also replace the use of a future entirely, for the case where you want to perform some operation after an asynchronous task completes.

You do this with the function doc://com.apple.documentation/documentation/swift/withCheckedContinuation(function:\_:) and its throwing equivalent, doc://com.apple.documentation/documentation/swift/swift/withCheckedThrowingContinuation(function:\_:). The following example performs the same asynchronous random number generation as the `Future` example above, but as an `async` method:

```
func generateAsyncRandomNumberFromContinuation() async -> Int {
    return await withCheckedContinuation { continuation in
        DispatchQueue.main.asyncAfter(deadline: .now() + 2) {
            let number = Int.random(in: 1...10)
            continuation.resume(returning: number)
        }
    }
}
```

The call point for this method doesn’t use a closure like the future’s sink subscriber does; it simply awaits and assigns the result:

```
let asyncRandom = await generateAsyncRandomNumberFromContinuation()
```

For more information on continuations, see the Concurrency topic in the Swift standard library.

## Topics

### Creating a Future

init((Future&lt;Output, Failure>.Promise) -> Void)

Creates a publisher that invokes a promise closure when the publisher emits an element.

typealias Promise

A type that represents a closure to invoke in the future, when an element or error is available.

### Accessing the Value Asynchronously

var value: Output

The published value of the future, delivered asynchronously.

var value: Output

The published value of the future or an error, delivered asynchronously.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Convenience Publishers

struct Just

A publisher that emits an output to each subscriber just once, and then finishes.

struct Deferred

A publisher that awaits subscription before running the supplied closure to create a publisher for the new subscriber.

struct Empty

A publisher that never publishes any values, and optionally finishes immediately.

struct Fail

A publisher that immediately terminates with the specified error.

struct Record

A publisher that allows for recording a series of inputs and a completion, for later playback to each subscriber.

