

- Combine
-  Subject 

Protocol

# Subject

A publisher that exposes a method for outside callers to publish elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol Subject : AnyObject, Publisher
```

## Mentioned in 

Using Combine for Your App’s Asynchronous Code

## Overview

A subject is a publisher that you can use to ”inject” values into a stream, by calling its send(_:) method. This can be useful for adapting existing imperative code to the Combine model.

## Topics

### Delivering Elements to Subscribers

func send(Self.Output)

Sends a value to the subscriber.

**Required**

func send()

Sends a void value to the subscriber.

### Delivering Life Cycle Events to Subscribers

func send(subscription: any Subscription)

Sends a subscription to the subscriber.

**Required**

func send(completion: Subscribers.Completion&lt;Self.Failure>)

Sends a completion signal to the subscriber.

**Required**

## Relationships

### Inherits From

- Publisher

### Conforming Types

- CurrentValueSubject
- PassthroughSubject

## See Also

### Subjects

class CurrentValueSubject

A subject that wraps a single value and publishes a new element whenever the value changes.

class PassthroughSubject

A subject that broadcasts elements to downstream subscribers.

