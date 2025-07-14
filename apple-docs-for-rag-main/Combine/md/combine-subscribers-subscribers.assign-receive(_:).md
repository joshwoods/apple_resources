

- Combine
- Subscribers
- Subscribers.Assign
-  receive(\_:) 

Instance Method

# receive(\_:)

Tells the subscriber that the publisher has produced an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func receive(_ value: Input) -> Subscribers.Demand
```

## Discussion

A Subscribers.Demand instance indicating how many more elements the subscriber expects to receive.

