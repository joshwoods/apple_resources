

- Combine
- Deferred
-  createPublisher 

Instance Property

# createPublisher

The closure to execute when this deferred publisher receives a subscription.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let createPublisher: () -> DeferredPublisher
```

## Discussion

The publisher returned by this closure immediately receives the incoming subscription.

