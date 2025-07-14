

- Combine
- Future
-  init(\_:) 

Initializer

# init(\_:)

Creates a publisher that invokes a promise closure when the publisher emits an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ attemptToFulfill: @escaping (@escaping Future.Promise) -> Void)
```

## Parameters 

`attemptToFulfill`  

A Future.Promise that the publisher invokes when the publisher emits an element or terminates with an error.

## See Also

### Creating a Future

typealias Promise

A type that represents a closure to invoke in the future, when an element or error is available.

