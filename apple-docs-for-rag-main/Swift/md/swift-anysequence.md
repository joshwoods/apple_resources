

- Swift
-  AnySequence 

Structure

# AnySequence

A type-erased sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct AnySequence
```

## Overview

An instance of `AnySequence` forwards its operations to an underlying base sequence having the same `Element` type, hiding the specifics of the underlying sequence.

## Topics

### Initializers

init&lt;I>(() -> I)

Creates a sequence whose `makeIterator()` method forwards to `makeUnderlyingIterator`.

init&lt;S>(S)

Creates a new sequence that wraps and forwards operations to `base`.

### Instance Methods

func drop(while: (Element) throws -> Bool) rethrows -> AnySequence&lt;Element>

func dropFirst(Int) -> AnySequence&lt;Element>

func dropLast(Int) -> [Element]

func filter((Element) throws -> Bool) rethrows -> [Element]

func forEach((Element) throws -> Void) rethrows

func map&lt;T, E>((Element) throws(E) -> T) throws(E) -> [T]

func prefix(Int) -> AnySequence&lt;Element>

func prefix(while: (Element) throws -> Bool) rethrows -> [Element]

func suffix(Int) -> [Element]

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

## See Also

### Type-Erasing Wrappers

struct AnyCollection

A type-erased wrapper over any collection with indices that support forward traversal.

struct AnyBidirectionalCollection

A type-erased wrapper over any collection with indices that support bidirectional traversal.

struct AnyRandomAccessCollection

A type-erased wrapper over any collection with indices that support random access traversal.

struct AnyIterator

A type-erased iterator of `Element`.

struct AnyIndex

A wrapper over an underlying index that hides the specific underlying type.

struct AnyHashable

A type-erased hashable value.

