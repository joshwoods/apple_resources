

- Combine
-  PassthroughSubject 

Class

# PassthroughSubject

A subject that broadcasts elements to downstream subscribers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class PassthroughSubject where Failure : Error
```

## Mentioned in 

Using Combine for Your App’s Asynchronous Code

## Overview

As a concrete implementation of Subject, the PassthroughSubject provides a convenient way to adapt existing imperative code to the Combine model.

Unlike CurrentValueSubject, a PassthroughSubject doesn’t have an initial value or a buffer of the most recently-published element. A PassthroughSubject drops values if there are no subscribers, or its current demand is zero.

## Topics

### Creating a Passthrough Subject

init()

### Delivering Elements to Subscribers

func send(Output)

Sends a value to the subscriber.

func send()

Sends a void value to the subscriber.

### Delivering Life Cycle Events to Subscribers

func send(subscription: any Subscription)

Sends a subscription to the subscriber.

func send(completion: Subscribers.Completion&lt;Failure>)

Sends a completion signal to the subscriber.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

Subject Implementations

## Relationships

### Conforms To

- Publisher
- Subject

## See Also

### Subjects

protocol Subject

A publisher that exposes a method for outside callers to publish elements.

class CurrentValueSubject

A subject that wraps a single value and publishes a new element whenever the value changes.

