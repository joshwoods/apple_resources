

- Combine
- Published
- Published.Publisher
-  receive(subscriber:) 

Instance Method

# receive(subscriber:)

Attaches the specified subscriber to this publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(subscriber: S) where Value == S.Input, S : Subscriber, S.Failure == Never
```

## Parameters 

`subscriber`  

The subscriber to attach to this Published.Publisher, after which it can receive values.

## Discussion

Implementations of Published.Publisher must implement this method.

The provided implementation of subscribe(_:)calls this method.

