

- Combine
- Publishers
-  Publishers.SetFailureType 

Structure

# Publishers.SetFailureType

A publisher that appears to send a specified failure type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SetFailureType where Upstream : Publisher, Failure : Error, Upstream.Failure == Never
```

## Overview

The publisher can’t actually fail with the specified type and finishes normally. Use this publisher type when you need to match the error types for two mismatched publishers.

## Topics

### Creating a Set Failure Type Publisher

init(upstream: Upstream)

Creates a publisher that appears to send a specified failure type.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

### Comparing Publishers

static func == (Publishers.SetFailureType&lt;Upstream, Failure>, Publishers.SetFailureType&lt;Upstream, Failure>) -> Bool

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

### Mapping Elements

struct Map

A publisher that transforms all elements from the upstream publisher with a provided closure.

struct TryMap

A publisher that transforms all elements from the upstream publisher with a provided error-throwing closure.

struct MapError

A publisher that converts any failure from the upstream publisher into a new error.

struct Scan

A publisher that transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

struct TryScan

A publisher that transforms elements from the upstream publisher by providing the current element to a failable closure along with the last value returned by the closure.

