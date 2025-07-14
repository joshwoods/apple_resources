

- Combine
- Future
-  Future.Promise 

Type Alias

# Future.Promise

A type that represents a closure to invoke in the future, when an element or error is available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Promise = (Result) -> Void
```

## Mentioned in 

Using Combine for Your App’s Asynchronous Code

## Discussion

The promise closure receives one parameter: a `Result` that contains either a single element published by a Future, or an error.

## See Also

### Creating a Future

init((Future&lt;Output, Failure>.Promise) -> Void)

Creates a publisher that invokes a promise closure when the publisher emits an element.

