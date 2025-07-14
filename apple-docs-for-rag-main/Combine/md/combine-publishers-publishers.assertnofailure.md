

- Combine
- Publishers
-  Publishers.AssertNoFailure 

Structure

# Publishers.AssertNoFailure

A publisher that raises a fatal error upon receiving any failure, and otherwise republishes all received input.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct AssertNoFailure where Upstream : Publisher
```

## Overview

Use this function for internal integrity checks that are active during testing but don’t affect performance of shipping code.

## Topics

### Creating an Assert No Failure Publisher

init(upstream: Upstream, prefix: String, file: StaticString, line: UInt)

Creates a publisher that raises a fatal error upon receiving any failure, and otherwise republishes all received input.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let file: StaticString

The filename used in the error message.

let line: UInt

The line number used in the error message.

let prefix: String

The string used at the beginning of the fatal error message.

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

struct Catch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

struct TryCatch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher or producing a new error.

struct Retry

A publisher that attempts to recreate its subscription to a failed upstream publisher.

