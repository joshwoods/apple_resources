

- Combine
- Publishers
-  Publishers.Print 

Structure

# Publishers.Print

A publisher that prints log messages for all publishing events, optionally prefixed with a given string.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Print where Upstream : Publisher
```

## Overview

This publisher prints log messages when receiving the following events:

- subscription

- value

- normal completion

- failure

- cancellation

## Topics

### Creating a Print Publisher

init(upstream: Upstream, prefix: String, to: (any TextOutputStream)?)

Creates a publisher that prints log messages for all publishing events.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let prefix: String

A string with which to prefix all log messages.

let stream: (any TextOutputStream)?

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

struct HandleEvents

A publisher that performs the specified closures when publisher events occur.

