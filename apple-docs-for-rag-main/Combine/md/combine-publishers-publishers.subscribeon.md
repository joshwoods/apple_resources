

- Combine
- Publishers
-  Publishers.SubscribeOn 

Structure

# Publishers.SubscribeOn

A publisher that receives elements from an upstream publisher on a specific scheduler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SubscribeOn where Upstream : Publisher, Context : Scheduler
```

## Topics

### Creating a Subscribe-On Publisher

init(upstream: Upstream, scheduler: Context, options: Context.SchedulerOptions?)

Creates a publisher that receives elements from an upstream publisher on a specific scheduler.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let scheduler: Context

The scheduler the publisher should use to receive elements.

let options: Context.SchedulerOptions?

Scheduler options that customize the delivery of elements.

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

struct ReceiveOn

A publisher that delivers elements to its downstream subscriber on a specific scheduler.

