

- Combine
- Publishers
-  Publishers.Retry 

Structure

# Publishers.Retry

A publisher that attempts to recreate its subscription to a failed upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Retry where Upstream : Publisher
```

## Topics

### Creating a Retry Publisher

init(upstream: Upstream, retries: Int?)

Creates a publisher that attempts to recreate its subscription to a failed upstream publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let retries: Int?

The maximum number of retry attempts to perform.

### Comparing Publishers

static func == (Publishers.Retry&lt;Upstream>, Publishers.Retry&lt;Upstream>) -> Bool

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

### Handling Errors

struct AssertNoFailure

A publisher that raises a fatal error upon receiving any failure, and otherwise republishes all received input.

struct Catch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

struct TryCatch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher or producing a new error.

