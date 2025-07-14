

- Combine
- Publishers
- Publishers.Breakpoint
-  receiveCompletion 

Instance Property

# receiveCompletion

A closure that executes when the publisher receives completion, and can raise a debugger signal by returning a true Boolean value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let receiveCompletion: ((Subscribers.Completion.Failure>) -> Bool)?
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let receiveSubscription: ((any Subscription) -> Bool)?

A closure that executes when the publisher receives a subscription, and can raise a debugger signal by returning a true Boolean value.

let receiveOutput: ((Upstream.Output) -> Bool)?

A closure that executes when the publisher receives output from the upstream publisher, and can raise a debugger signal by returning a true Boolean value.

