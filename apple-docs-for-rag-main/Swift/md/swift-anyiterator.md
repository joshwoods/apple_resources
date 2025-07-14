

- Swift
-  AnyIterator 

Structure

# AnyIterator

A type-erased iterator of `Element`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct AnyIterator
```

## Overview

This iterator forwards its `next()` method to an arbitrary underlying iterator having the same `Element` type, hiding the specifics of the underlying `IteratorProtocol`.

## Topics

### Initializers

init&lt;I>(I)

Creates an iterator that wraps a base iterator but whose type depends only on the base iterator’s element type.

init(() -> Element?)

Creates an iterator that wraps the given closure in its `next()` method.

### Default Implementations

IteratorProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- IteratorProtocol

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

## See Also

### Type-Erasing Wrappers

struct AnySequence

A type-erased sequence.

struct AnyCollection

A type-erased wrapper over any collection with indices that support forward traversal.

struct AnyBidirectionalCollection

A type-erased wrapper over any collection with indices that support bidirectional traversal.

struct AnyRandomAccessCollection

A type-erased wrapper over any collection with indices that support random access traversal.

struct AnyIndex

A wrapper over an underlying index that hides the specific underlying type.

struct AnyHashable

A type-erased hashable value.

