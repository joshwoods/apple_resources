

- Combine
- Publishers
-  Publishers.Breakpoint 

Structure

# Publishers.Breakpoint

A publisher that raises a debugger signal when a provided closure needs to stop the process in the debugger.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Breakpoint where Upstream : Publisher
```

## Overview

When any of the provided closures returns `true`, this publisher raises the `SIGTRAP` signal to stop the process in the debugger. Otherwise, this publisher passes through values and completions as-is.

## Topics

### Creating a Breakpoint Publisher

init(upstream: Upstream, receiveSubscription: ((any Subscription) -> Bool)?, receiveOutput: ((Upstream.Output) -> Bool)?, receiveCompletion: ((Subscribers.Completion&lt;Publishers.Breakpoint&lt;Upstream>.Failure>) -> Bool)?)

Creates a breakpoint publisher with the provided upstream publisher and breakpoint-raising closures.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let receiveSubscription: ((any Subscription) -> Bool)?

A closure that executes when the publisher receives a subscription, and can raise a debugger signal by returning a true Boolean value.

let receiveOutput: ((Upstream.Output) -> Bool)?

A closure that executes when the publisher receives output from the upstream publisher, and can raise a debugger signal by returning a true Boolean value.

let receiveCompletion: ((Subscribers.Completion&lt;Publishers.Breakpoint&lt;Upstream>.Failure>) -> Bool)?

A closure that executes when the publisher receives completion, and can raise a debugger signal by returning a true Boolean value.

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

struct HandleEvents

A publisher that performs the specified closures when publisher events occur.

struct Print

A publisher that prints log messages for all publishing events, optionally prefixed with a given string.

