

- Combine
- Publishers
-  Publishers.TryCatch 

Structure

# Publishers.TryCatch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher or producing a new error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct TryCatch where Upstream : Publisher, NewPublisher : Publisher, Upstream.Output == NewPublisher.Output
```

## Overview

Because this publisher’s handler can throw an error, Publishers.TryCatch defines its Failure type as `Error`. This is different from Publishers.Catch, which gets its failure type from the replacement publisher.

## Topics

### Creating a Try-Catch Publisher

init(upstream: Upstream, handler: (Upstream.Failure) throws -> NewPublisher)

Creates a publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher or by throwing an error.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives its elements.

let handler: (Upstream.Failure) throws -> NewPublisher

A closure that accepts the upstream failure as input and either returns a publisher to replace the upstream publisher or throws an error.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Handling Errors

struct AssertNoFailure

A publisher that raises a fatal error upon receiving any failure, and otherwise republishes all received input.

struct Catch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

struct Retry

A publisher that attempts to recreate its subscription to a failed upstream publisher.

