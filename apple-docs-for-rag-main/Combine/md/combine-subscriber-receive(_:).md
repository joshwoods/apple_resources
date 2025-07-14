

- Combine
- Subscriber
-  receive(\_:) 

Instance Method

# receive(\_:)

Tells the subscriber that the publisher has produced an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(_ input: Self.Input) -> Subscribers.Demand
```

**Required**

## Parameters 

`input`  

The published element.

## Return Value

A `Subscribers.Demand` instance indicating how many more elements the subscriber expects to receive.

## Mentioned in 

Processing Published Elements with Subscribers

## See Also

### Receiving Elements

func receive() -> Subscribers.Demand

Tells the subscriber that a publisher of void elements is ready to receive further requests.

