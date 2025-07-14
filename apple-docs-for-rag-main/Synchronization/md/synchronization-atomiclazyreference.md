

- Synchronization
-  AtomicLazyReference 

Structure

# AtomicLazyReference

A lazily initializable atomic strong reference.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct AtomicLazyReference where Instance : AnyObject
```

## Overview

These values can be set (initialized) exactly once, but read many times.

## Topics

### Initializers

init()

### Instance Methods

func load() -> Instance?

Atomically loads and returns the current value of this reference.

func storeIfNil(consuming Instance) -> Instance

Atomically initializes this reference if its current value is nil, then returns the initialized value. If this reference is already initialized, then `storeIfNil(_:)` discards its supplied argument and returns the current value without updating it.

## Relationships

### Conforms To

- Sendable

  Conforms when `Instance` conforms to `Copyable`, `Escapable`, and `Sendable`.

## See Also

### Atomic Values

struct Atomic

An atomic value.

struct WordPair

A pair of two word sized `UInt`s.

protocol AtomicRepresentable

A type that supports atomic operations through a separate atomic storage representation.

protocol AtomicOptionalRepresentable

An atomic value that also supports atomic operations when wrapped in an `Optional`. Atomic optional representable types come with a standalone atomic representation for their optional-wrapped variants.

