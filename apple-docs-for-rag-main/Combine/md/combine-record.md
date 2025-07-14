

- Combine
-  Record 

Structure

# Record

A publisher that allows for recording a series of inputs and a completion, for later playback to each subscriber.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Record where Failure : Error
```

## Topics

### Creating a Record Publisher

init(output: [Output], completion: Subscribers.Completion&lt;Failure>)

Creates a record publisher to publish the provided elements, followed by the provided completion value.

init(record: (inout Record&lt;Output, Failure>.Recording) -> Void)

Creates a publisher to interactively record a series of outputs and a completion.

init(recording: Record&lt;Output, Failure>.Recording)

Creates a record publisher from an existing recording.

### Inspecting Publisher Properties

let recording: Record&lt;Output, Failure>.Recording

The recorded output and completion.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Structures

struct Recording

A recorded sequence of outputs, followed by a completion value.

### Default Implementations

Decodable Implementations

Encodable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
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

struct Fail

A publisher that immediately terminates with the specified error.

