

- Swift
-  AnyCollection 

Structure

# AnyCollection

A type-erased wrapper over any collection with indices that support forward traversal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct AnyCollection
```

## Overview

An `AnyCollection` instance forwards its operations to a base collection having the same `Element` type, hiding the specifics of the underlying collection.

## Topics

### Initializers

init(AnyCollection&lt;Element>)

Creates an `AnyCollection` having the same underlying collection as `other`.

init&lt;C>(C)

Creates a type-erased collection that wraps the given collection.

init(AnyBidirectionalCollection&lt;Element>)

Creates an `AnyCollection` having the same underlying collection as `other`.

init&lt;C>(C)

Creates a type-erased collection that wraps the given collection.

init(AnyRandomAccessCollection&lt;Element>)

Creates an `AnyCollection` having the same underlying collection as `other`.

init&lt;C>(C)

Creates a type-erased collection that wraps the given collection.

### Instance Methods

func drop(while: (Element) throws -> Bool) rethrows -> AnyCollection&lt;Element>

func dropFirst(Int) -> AnyCollection&lt;Element>

func dropLast(Int) -> AnyCollection&lt;Element>

func filter((Element) throws -> Bool) rethrows -> [Element]

func forEach((Element) throws -> Void) rethrows

func formIndex(inout AnyCollection&lt;Element>.Index, offsetBy: Int)

func formIndex(inout AnyCollection&lt;Element>.Index, offsetBy: Int, limitedBy: AnyCollection&lt;Element>.Index) -> Bool

func map&lt;T, E>((Element) throws(E) -> T) throws(E) -> [T]

func prefix(Int) -> AnyCollection&lt;Element>

func prefix(while: (Element) throws -> Bool) rethrows -> AnyCollection&lt;Element>

func suffix(Int) -> AnyCollection&lt;Element>

### Default Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

## See Also

### Type-Erasing Wrappers

struct AnySequence

A type-erased sequence.

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

