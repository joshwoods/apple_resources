

- Combine
- Publishers
-  Publishers.Multicast 

Class

# Publishers.Multicast

A publisher that uses a subject to deliver elements to multiple subscribers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class Multicast where Upstream : Publisher, SubjectType : Subject, Upstream.Failure == SubjectType.Failure, Upstream.Output == SubjectType.Output
```

## Mentioned in 

Controlling Publishing with Connectable Publishers

## Overview

Use a multicast publisher when you have multiple downstream subscribers, but you want upstream publishers to only process one receive(_:) call per event.

## Topics

### Creating a Multicast Publisher

init(upstream: Upstream, createSubject: () -> SubjectType)

Creates a multicast publisher that applies a closure to create a subject that delivers elements to subscribers.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives its elements.

let createSubject: () -> SubjectType

A closure that returns a subject each time a subscriber attaches to the multicast publisher.

### Performing Explicit Connections

func connect() -> any Cancellable

Connects to the publisher, allowing it to produce elements, and returns an instance with which to cancel publishing.

### Connecting Automatically

func autoconnect() -> Publishers.Autoconnect&lt;Self>

Automates the process of connecting or disconnecting from this connectable publisher.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

ConnectablePublisher Implementations

Publisher Implementations

## Relationships

### Conforms To

- ConnectablePublisher
- Publisher

## See Also

### Working with Multiple Subscribers

class Share

A publisher that shares the output of an upstream publisher with multiple subscribers.

