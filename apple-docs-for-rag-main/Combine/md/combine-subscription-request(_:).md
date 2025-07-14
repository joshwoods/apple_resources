

- Combine
- Subscription
-  request(\_:) 

Instance Method

# request(\_:)

Tells a publisher that it may send more values to the subscriber.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func request(_ demand: Subscribers.Demand)
```

**Required**

## Mentioned in 

Processing Published Elements with Subscribers

## See Also

### Requesting Elements

struct Demand

A requested number of items, sent to a publisher from a subscriber through the subscription.

