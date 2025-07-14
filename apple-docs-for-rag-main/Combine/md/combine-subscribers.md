

- Combine
-  Subscribers 

Enumeration

# Subscribers

A namespace for types that serve as subscribers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Subscribers
```

## Topics

### Requesting Elements

struct Demand

A requested number of items, sent to a publisher from a subscriber through the subscription.

### Receiving Life Cycle Events

enum Completion

A signal that a publisher doesn’t produce additional elements, either due to normal completion or an error.

### Using Convenience Subscribers

class Sink

A simple subscriber that requests an unlimited number of values upon subscription.

class Assign

A simple subscriber that assigns received elements to a property indicated by a key path.

## See Also

### Subscribers

Processing Published Elements with Subscribers

Apply back pressure to precisely control when publishers produce elements.

protocol Subscriber

A protocol that declares a type that can receive input from a publisher.

struct AnySubscriber

A type-erasing subscriber.

protocol Subscription

A protocol representing the connection of a subscriber to a publisher.

enum Subscriptions

A namespace for symbols related to subscriptions.

