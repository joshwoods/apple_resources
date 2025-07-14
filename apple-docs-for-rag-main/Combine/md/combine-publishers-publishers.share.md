

- Combine
- Publishers
-  Publishers.Share 

Class

# Publishers.Share

A publisher that shares the output of an upstream publisher with multiple subscribers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class Share where Upstream : Publisher
```

## Overview

This publisher type supports multiple subscribers, all of whom receive unchanged elements and completion states from the upstream publisher.

Tip

Publishers.Share is effectively a combination of the Publishers.Multicast and PassthroughSubject publishers, with an implicit autoconnect().

Be aware that Publishers.Share is a class rather than a structure like most other publishers. Use this type when you need a publisher instance that uses reference semantics.

## Topics

### Creating a Share Publisher

init(upstream: Upstream)

Creates a publisher that shares the output of an upstream publisher with multiple subscribers.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

### Comparing Publishers

static func == (Publishers.Share&lt;Upstream>, Publishers.Share&lt;Upstream>) -> Bool

Returns a Boolean value that indicates whether two publishers are equivalent.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Equatable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Equatable
- Publisher

## See Also

### Working with Multiple Subscribers

class Multicast

A publisher that uses a subject to deliver elements to multiple subscribers.

