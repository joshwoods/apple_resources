

- Combine
-  AnyCancellable 

Class

# AnyCancellable

A type-erasing cancellable object that executes a provided closure when canceled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class AnyCancellable
```

## Mentioned in 

Controlling Publishing with Connectable Publishers

## Overview

Subscriber implementations can use this type to provide a “cancellation token” that makes it possible for a caller to cancel a publisher, but not to use the Subscription object to request items.

An AnyCancellable instance automatically calls cancel() when deinitialized.

## Topics

### Creating a Type-Erased Cancellable

init(() -> Void)

Initializes the cancellable object with the given cancel-time closure.

### Canceling Actions

func cancel()

Cancel the activity.

### Storing AnyCancellable Instances

func store&lt;C>(in: inout C)

Stores this type-erasing cancellable instance in the specified collection.

func store(in: inout Set&lt;AnyCancellable>)

Stores this type-erasing cancellable instance in the specified set.

### Operators

static func == (AnyCancellable, AnyCancellable) -> Bool

Returns a Boolean value that indicates whether two instances are equal, as determined by comparing whether their references point to the same instance.

### Initializers

init&lt;C>(C)

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Cancellable
- Equatable
- Hashable

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

protocol Cancellable

A protocol indicating that an activity or action supports cancellation.

