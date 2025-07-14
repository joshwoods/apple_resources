

- Combine
- Subscribers
- Subscribers.Sink
-  init(receiveCompletion:receiveValue:) 

Initializer

# init(receiveCompletion:receiveValue:)

Initializes a sink with the provided closures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    receiveCompletion: @escaping (Subscribers.Completion) -> Void,
    receiveValue: @escaping (Input) -> Void
)
```

## Parameters 

`receiveCompletion`  

The closure to execute on completion.

`receiveValue`  

The closure to execute on receipt of a value.

