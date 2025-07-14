

- Dispatch
-  DispatchPredicate 

Enumeration

# DispatchPredicate

Logical conditions to evaluate within a given execution context.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
enum DispatchPredicate
```

## Overview

You use dispatch predicates with the dispatchPrecondition(condition:) method.

## Topics

### Predicates

case onQueue(DispatchQueue)

A predicate that indicates the evaluated context is the associated dispatch queue.

case onQueueAsBarrier(DispatchQueue)

A predicate that indicates the evaluated context is the associated dispatch queue as part of a barrier operation.

case notOnQueue(DispatchQueue)

A predicate that indicates the evaluated context is not the associated dispatch queue.

## Relationships

### Conforms To

- Sendable

## See Also

### Dispatch Objects

class DispatchObject

The base class for most dispatch types.

func dispatchPrecondition(condition: @autoclosure () -> DispatchPredicate)

Checks a dispatch condition necessary for further execution.

Dispatch Objects

The basic behaviors supported by all dispatch types.

