

- Swift
- Optional
- Optional.Publisher
-  receive(subscriber:) 

Instance Method

# receive(subscriber:)

Implements the Publisher protocol by accepting the subscriber and immediately publishing the optional’s value if it has one, or finishing normally if it doesn’t.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(subscriber: S) where Wrapped == S.Input, S : Subscriber, S.Failure == Never
```

## Parameters 

`subscriber`  

The subscriber to add.

