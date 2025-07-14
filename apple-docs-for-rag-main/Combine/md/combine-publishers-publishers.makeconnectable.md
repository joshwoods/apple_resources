

- Combine
- Publishers
-  Publishers.MakeConnectable 

Structure

# Publishers.MakeConnectable

A publisher that provides explicit connectability to another publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct MakeConnectable where Upstream : Publisher
```

## Mentioned in 

Controlling Publishing with Connectable Publishers

## Overview

Publishers.MakeConnectable is a ConnectablePublisher, which allows you to perform configuration before publishing any elements. Call connect() on this publisher when you want to attach to its upstream publisher and start producing elements.

Use the makeConnectable() operator to wrap an upstream publisher with an instance of this publisher.

## Topics

### Creating a Connectable Publisher

init(upstream: Upstream)

Creates a connectable publisher, attached to the provide upstream publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

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

### Using Explicit Publisher Connections

class Autoconnect

A publisher that automatically connects to an upstream connectable publisher.

