

- Combine
-  Subscription 

Protocol

# Subscription

A protocol representing the connection of a subscriber to a publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol Subscription : Cancellable, CustomCombineIdentifierConvertible
```

## Mentioned in 

Receiving and Handling Events with Combine

Processing Published Elements with Subscribers

## Overview

Subscriptions are class constrained because a Subscription has identity, defined by the moment in time a particular subscriber attached to a publisher. Canceling a Subscription must be thread-safe.

You can only cancel a Subscription once.

Canceling a subscription frees up any resources previously allocated by attaching the Subscriber.

## Topics

### Requesting Elements

func request(Subscribers.Demand)

Tells a publisher that it may send more values to the subscriber.

**Required**

struct Demand

A requested number of items, sent to a publisher from a subscriber through the subscription.

## Relationships

### Inherits From

- Cancellable
- CustomCombineIdentifierConvertible

## See Also

### Subscribers

Processing Published Elements with Subscribers

Apply back pressure to precisely control when publishers produce elements.

protocol Subscriber

A protocol that declares a type that can receive input from a publisher.

enum Subscribers

A namespace for types that serve as subscribers.

struct AnySubscriber

A type-erasing subscriber.

enum Subscriptions

A namespace for symbols related to subscriptions.

