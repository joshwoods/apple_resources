

- Combine
-  ConnectablePublisher 

Protocol

# ConnectablePublisher

A publisher that provides an explicit means of connecting and canceling publication.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol ConnectablePublisher : Publisher
```

## Mentioned in 

Controlling Publishing with Connectable Publishers

Replacing Foundation Timers with Timer Publishers

## Overview

Use a ConnectablePublisher when you need to perform additional configuration or setup prior to producing any elements.

This publisher doesn’t produce any elements until you call its connect() method.

Use makeConnectable() to create a ConnectablePublisher from any publisher whose failure type is Never.

## Topics

### Performing Explicit Connections

func connect() -> any Cancellable

Connects to the publisher, allowing it to produce elements, and returns an instance with which to cancel publishing.

**Required**

### Connecting Automatically

func autoconnect() -> Publishers.Autoconnect&lt;Self>

Automates the process of connecting or disconnecting from this connectable publisher.

## Relationships

### Inherits From

- Publisher

### Conforming Types

- Publishers.MakeConnectable
- Publishers.Multicast

## See Also

### Connectable Publishers

Controlling Publishing with Connectable Publishers

Coordinate when publishers start sending elements to subscribers.

