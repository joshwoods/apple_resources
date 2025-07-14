

- Combine
- Publishers
-  Publishers.HandleEvents 

Structure

# Publishers.HandleEvents

A publisher that performs the specified closures when publisher events occur.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct HandleEvents where Upstream : Publisher
```

## Topics

### Creating a HandleEvents Publisher

init(upstream: Upstream, receiveSubscription: ((any Subscription) -> Void)?, receiveOutput: ((Publishers.HandleEvents&lt;Upstream>.Output) -> Void)?, receiveCompletion: ((Subscribers.Completion&lt;Publishers.HandleEvents&lt;Upstream>.Failure>) -> Void)?, receiveCancel: (() -> Void)?, receiveRequest: ((Subscribers.Demand) -> Void)?)

Creates a publisher that performs the specified closures when publisher events occur.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

var receiveSubscription: ((any Subscription) -> Void)?

A closure that executes when the publisher receives the subscription from the upstream publisher.

var receiveOutput: ((Publishers.HandleEvents&lt;Upstream>.Output) -> Void)?

A closure that executes when the publisher receives a value from the upstream publisher.

var receiveCompletion: ((Subscribers.Completion&lt;Publishers.HandleEvents&lt;Upstream>.Failure>) -> Void)?

A closure that executes when the upstream publisher finishes normally or terminates with an error.

var receiveCancel: (() -> Void)?

A closure that executes when the downstream receiver cancels publishing.

var receiveRequest: ((Subscribers.Demand) -> Void)?

A closure that executes when the publisher receives a request for more elements.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Debugging

struct Breakpoint

A publisher that raises a debugger signal when a provided closure needs to stop the process in the debugger.

struct Print

A publisher that prints log messages for all publishing events, optionally prefixed with a given string.

