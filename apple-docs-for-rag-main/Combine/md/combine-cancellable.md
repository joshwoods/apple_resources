

- Combine
-  Cancellable 

Protocol

# Cancellable

A protocol indicating that an activity or action supports cancellation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol Cancellable
```

## Mentioned in 

Receiving and Handling Events with Combine

Controlling Publishing with Connectable Publishers

## Overview

Calling cancel() frees up any allocated resources. It also stops side effects such as timers, network access, or disk I/O.

## Topics

### Canceling Actions

func cancel()

Cancel the activity.

**Required**

### Storing Cancellable Instances

func store&lt;C>(in: inout C)

Stores this cancellable instance in the specified collection.

func store(in: inout Set&lt;AnyCancellable>)

Stores this cancellable instance in the specified set.

### Instance Methods

func storeWhileEntityActive(Entity)

Retains the `Cancellable` as long as the entity is active (see `Entity.isActive`). If the entity is deactivated, the `Cancellable` is released.

## Relationships

### Inherited By

- Subscription

### Conforming Types

- AnyCancellable
- Subscribers.Assign
- Subscribers.Sink

## See Also

### Publishers

protocol Publisher

Declares that a type can transmit a sequence of values over time.

enum Publishers

A namespace for types that serve as publishers.

struct AnyPublisher

A publisher that performs type erasure by wrapping another publisher.

struct Published

A type that publishes a property marked with an attribute.

class AnyCancellable

A type-erasing cancellable object that executes a provided closure when canceled.

