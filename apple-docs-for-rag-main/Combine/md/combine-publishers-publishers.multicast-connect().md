

- Combine
- Publishers
- Publishers.Multicast
-  connect() 

Instance Method

# connect()

Connects to the publisher, allowing it to produce elements, and returns an instance with which to cancel publishing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func connect() -> any Cancellable
```

## Return Value

A Cancellable instance that you use to cancel publishing.

