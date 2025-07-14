

- Combine
- Publishers
-  Publishers.ReceiveOn 

Structure

# Publishers.ReceiveOn

A publisher that delivers elements to its downstream subscriber on a specific scheduler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ReceiveOn where Upstream : Publisher, Context : Scheduler
```

## Topics

### Creating a Receive-On Publisher

init(upstream: Upstream, scheduler: Context, options: Context.SchedulerOptions?)

Creates a publisher that delivers elements to its downstream subscriber on a specific scheduler.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let scheduler: Context

The scheduler the publisher uses to deliver elements.

let options: Context.SchedulerOptions?

Scheduler options used to customize element delivery.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Working with Subscribers

struct SubscribeOn

A publisher that receives elements from an upstream publisher on a specific scheduler.

