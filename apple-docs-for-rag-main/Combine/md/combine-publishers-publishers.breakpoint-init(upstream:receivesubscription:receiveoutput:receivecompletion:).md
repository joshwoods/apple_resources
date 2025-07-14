

- Combine
- Publishers
- Publishers.Breakpoint
-  init(upstream:receiveSubscription:receiveOutput:receiveCompletion:) 

Initializer

# init(upstream:receiveSubscription:receiveOutput:receiveCompletion:)

Creates a breakpoint publisher with the provided upstream publisher and breakpoint-raising closures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    receiveSubscription: ((any Subscription) -> Bool)? = nil,
    receiveOutput: ((Upstream.Output) -> Bool)? = nil,
    receiveCompletion: ((Subscribers.Completion.Failure>) -> Bool)? = nil
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`receiveSubscription`  

A closure that executes when the publisher receives a subscription, and can raise a debugger signal by returning a true Boolean value.

`receiveOutput`  

A closure that executes when the publisher receives output from the upstream publisher, and can raise a debugger signal by returning a true Boolean value.

`receiveCompletion`  

A closure that executes when the publisher receives completion, and can raise a debugger signal by returning a true Boolean value.

