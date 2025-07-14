

- Combine
-  Deferred 

Structure

# Deferred

A publisher that awaits subscription before running the supplied closure to create a publisher for the new subscriber.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Deferred where DeferredPublisher : Publisher
```

## Topics

### Creating a Deferred Publisher

init(createPublisher: () -> DeferredPublisher)

Creates a deferred publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let createPublisher: () -> DeferredPublisher

The closure to execute when this deferred publisher receives a subscription.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Convenience Publishers

class Future

A publisher that eventually produces a single value and then finishes or fails.

struct Just

A publisher that emits an output to each subscriber just once, and then finishes.

struct Empty

A publisher that never publishes any values, and optionally finishes immediately.

struct Fail

A publisher that immediately terminates with the specified error.

struct Record

A publisher that allows for recording a series of inputs and a completion, for later playback to each subscriber.

