

- Synchronization
-  Mutex 

Structure

# Mutex

A synchronization primitive that protects shared mutable state via mutual exclusion.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct Mutex where Value : ~Copyable
```

## Overview

The `Mutex` type offers non-recursive exclusive access to the state it is protecting by blocking threads attempting to acquire the lock. Only one execution context at a time has access to the value stored within the `Mutex` allowing for exclusive access.

An example use of `Mutex` in a class used simultaneously by many threads protecting a `Dictionary` value:

```
class Manager {
  let cache = Mutex([:])

  func saveResource(_ resource: Resource, as key: Key) {
    cache.withLock {
      $0[key] = resource
    }
  }
}
```

## Topics

### Initializers

init(consuming sending Value)

Initializes a value of this mutex with the given initial state.

### Instance Methods

func withLock&lt;Result, E>((inout sending Value) throws(E) -> sending Result) throws(E) -> sending Result

Calls the given closure after acquiring the lock and then releases ownership.

func withLockIfAvailable&lt;Result, E>((inout sending Value) throws(E) -> sending Result) throws(E) -> sending Result?

Attempts to acquire the lock and then calls the given closure if successful.

## Relationships

### Conforms To

- Sendable

  Conforms when `Value` conforms to `Escapable`.

