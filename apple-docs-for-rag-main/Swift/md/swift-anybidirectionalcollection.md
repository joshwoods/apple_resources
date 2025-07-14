

- Swift
-  AnyBidirectionalCollection 

Structure

# AnyBidirectionalCollection

A type-erased wrapper over any collection with indices that support bidirectional traversal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct AnyBidirectionalCollection
```

## Overview

An `AnyBidirectionalCollection` instance forwards its operations to a base collection having the same `Element` type, hiding the specifics of the underlying collection.

## Topics

### Initializers

init?(AnyCollection&lt;Element>)

Creates an `AnyBidirectionalCollection` having the same underlying collection as `other`.

init&lt;C>(C)

Creates a type-erased collection that wraps the given collection.

init(AnyRandomAccessCollection&lt;Element>)

Creates an `AnyBidirectionalCollection` having the same underlying collection as `other`.

init&lt;C>(C)

Creates a type-erased collection that wraps the given collection.

init(AnyBidirectionalCollection&lt;Element>)

Creates an `AnyBidirectionalCollection` having the same underlying collection as `other`.

### Instance Methods

func drop(while: (Element) throws -> Bool) rethrows -> AnyBidirectionalCollection&lt;Element>

func dropFirst(Int) -> AnyBidirectionalCollection&lt;Element>

func dropLast(Int) -> AnyBidirectionalCollection&lt;Element>

func filter((Element) throws -> Bool) rethrows -> [Element]

func forEach((Element) throws -> Void) rethrows

func formIndex(inout AnyBidirectionalCollection&lt;Element>.Index, offsetBy: Int)

func formIndex(inout AnyBidirectionalCollection&lt;Element>.Index, offsetBy: Int, limitedBy: AnyBidirectionalCollection&lt;Element>.Index) -> Bool

func map&lt;T, E>((Element) throws(E) -> T) throws(E) -> [T]

func prefix(Int) -> AnyBidirectionalCollection&lt;Element>

func prefix(while: (Element) throws -> Bool) rethrows -> AnyBidirectionalCollection&lt;Element>

func suffix(Int) -> AnyBidirectionalCollection&lt;Element>

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

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

struct AnyCollection

A type-erased wrapper over any collection with indices that support forward traversal.

struct AnyRandomAccessCollection

A type-erased wrapper over any collection with indices that support random access traversal.

struct AnyIterator

A type-erased iterator of `Element`.

struct AnyIndex

A wrapper over an underlying index that hides the specific underlying type.

struct AnyHashable

A type-erased hashable value.

