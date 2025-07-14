

- Combine
- Publishers
- Publishers.HandleEvents
-  receiveCompletion 

Instance Property

# receiveCompletion

A closure that executes when the upstream publisher finishes normally or terminates with an error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var receiveCompletion: ((Subscribers.Completion.Failure>) -> Void)?
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

var receiveSubscription: ((any Subscription) -> Void)?

A closure that executes when the publisher receives the subscription from the upstream publisher.

var receiveOutput: ((Publishers.HandleEvents&lt;Upstream>.Output) -> Void)?

A closure that executes when the publisher receives a value from the upstream publisher.

var receiveCancel: (() -> Void)?

A closure that executes when the downstream receiver cancels publishing.

var receiveRequest: ((Subscribers.Demand) -> Void)?

A closure that executes when the publisher receives a request for more elements.

