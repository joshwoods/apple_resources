

- Combine
-  Fail 

Structure

# Fail

A publisher that immediately terminates with the specified error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Fail where Failure : Error
```

## Topics

### Creating a Fail Publisher

init(error: Failure)

Creates a publisher that immediately terminates with the specified failure.

init(outputType: Output.Type, failure: Failure)

Creates publisher with the given output type, that immediately terminates with the specified failure.

### Inspecting Publisher Properties

let error: Failure

The failure to send when terminating the publisher.

### Comparing Publishers

static func == (Fail&lt;Output, Failure>, Fail&lt;Output, Failure>) -> Bool

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

- Copyable
- Equatable
- Publisher

## See Also

### Convenience Publishers

class Future

A publisher that eventually produces a single value and then finishes or fails.

struct Just

A publisher that emits an output to each subscriber just once, and then finishes.

struct Deferred

A publisher that awaits subscription before running the supplied closure to create a publisher for the new subscriber.

struct Empty

A publisher that never publishes any values, and optionally finishes immediately.

struct Record

A publisher that allows for recording a series of inputs and a completion, for later playback to each subscriber.

