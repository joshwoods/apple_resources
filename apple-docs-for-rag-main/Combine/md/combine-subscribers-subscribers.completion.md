

- Combine
- Subscribers
-  Subscribers.Completion 

Enumeration

# Subscribers.Completion

A signal that a publisher doesn’t produce additional elements, either due to normal completion or an error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
enum Completion where Failure : Error
```

## Mentioned in 

Receiving and Handling Events with Combine

## Topics

### Completion States

case finished

The publisher finished normally.

case failure(Failure)

The publisher stopped publishing due to the indicated error.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Receiving Life Cycle Events

func receive(subscription: any Subscription)

Tells the subscriber that it has successfully subscribed to the publisher and may request items.

**Required**

func receive(completion: Subscribers.Completion&lt;Self.Failure>)

Tells the subscriber that the publisher has completed publishing, either normally or with an error.

**Required**

