

- Combine
- Publishers
- Publishers.HandleEvents
-  receiveCancel 

Instance Property

# receiveCancel

A closure that executes when the downstream receiver cancels publishing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var receiveCancel: (() -> Void)?
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

var receiveSubscription: ((any Subscription) -> Void)?

A closure that executes when the publisher receives the subscription from the upstream publisher.

var receiveOutput: ((Publishers.HandleEvents&lt;Upstream>.Output) -> Void)?

A closure that executes when the publisher receives a value from the upstream publisher.

var receiveCompletion: ((Subscribers.Completion&lt;Publishers.HandleEvents&lt;Upstream>.Failure>) -> Void)?

A closure that executes when the upstream publisher finishes normally or terminates with an error.

var receiveRequest: ((Subscribers.Demand) -> Void)?

A closure that executes when the publisher receives a request for more elements.

