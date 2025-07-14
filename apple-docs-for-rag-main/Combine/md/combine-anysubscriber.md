

- Combine
-  AnySubscriber 

Structure

# AnySubscriber

A type-erasing subscriber.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct AnySubscriber where Failure : Error
```

## Overview

Use an AnySubscriber to wrap an existing subscriber whose details you don’t want to expose. You can also use AnySubscriber to create a custom subscriber by providing closures for the methods defined in Subscriber, rather than implementing Subscriber directly.

## Topics

### Creating a Type-Erased Subscriber

init&lt;S>(S)

Creates a type-erasing subscriber to wrap an existing subscriber.

init(receiveSubscription: ((any Subscription) -> Void)?, receiveValue: ((Input) -> Subscribers.Demand)?, receiveCompletion: ((Subscribers.Completion&lt;Failure>) -> Void)?)

Creates a type-erasing subscriber that executes the provided closures.

### Receiving Elements

func receive(Input) -> Subscribers.Demand

Tells the subscriber that the publisher has produced an element.

func receive() -> Subscribers.Demand

Tells the subscriber that a publisher of void elements is ready to receive further requests.

### Receiving Life Cycle Events

func receive(subscription: any Subscription)

Tells the subscriber that it has successfully subscribed to the publisher and may request items.

func receive(completion: Subscribers.Completion&lt;Failure>)

Tells the subscriber that the publisher has completed publishing, either normally or with an error.

### Inspecting Subscriber Properties

let combineIdentifier: CombineIdentifier

A unique identifier for identifying publisher streams.

var customMirror: Mirror

The custom mirror for this instance.

var description: String

A textual representation of this instance.

var playgroundDescription: Any

A custom playground description for this instance.

### Initializers

init&lt;S>(S)

Creates a type-erasing subscriber to wrap an existing subscriber.

### Default Implementations

Subscriber Implementations

## Relationships

### Conforms To

- CustomCombineIdentifierConvertible
- CustomPlaygroundDisplayConvertible
- CustomReflectable
- CustomStringConvertible
- Subscriber

## See Also

### Subscribers

Processing Published Elements with Subscribers

Apply back pressure to precisely control when publishers produce elements.

protocol Subscriber

A protocol that declares a type that can receive input from a publisher.

enum Subscribers

A namespace for types that serve as subscribers.

protocol Subscription

A protocol representing the connection of a subscriber to a publisher.

enum Subscriptions

A namespace for symbols related to subscriptions.

