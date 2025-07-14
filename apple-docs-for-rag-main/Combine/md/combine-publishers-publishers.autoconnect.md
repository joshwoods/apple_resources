

- Combine
- Publishers
-  Publishers.Autoconnect 

Class

# Publishers.Autoconnect

A publisher that automatically connects to an upstream connectable publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class Autoconnect where Upstream : ConnectablePublisher
```

## Overview

This publisher calls connect() on the upstream ConnectablePublisher when first attached to by a subscriber.

## Topics

### Creating an Autoconnect Publisher

init(upstream: Upstream)

Creates a publisher that automatically connects to an upstream connectable publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Using Explicit Publisher Connections

struct MakeConnectable

A publisher that provides explicit connectability to another publisher.

