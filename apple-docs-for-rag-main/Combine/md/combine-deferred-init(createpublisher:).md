

- Combine
- Deferred
-  init(createPublisher:) 

Initializer

# init(createPublisher:)

Creates a deferred publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(createPublisher: @escaping () -> DeferredPublisher)
```

## Parameters 

`createPublisher`  

The closure to execute when calling `subscribe(_:)`.

