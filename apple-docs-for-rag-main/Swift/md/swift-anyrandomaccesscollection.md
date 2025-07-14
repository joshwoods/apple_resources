

- Swift
-  AnyRandomAccessCollection 

Structure

# AnyRandomAccessCollection

A type-erased wrapper over any collection with indices that support random access traversal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct AnyRandomAccessCollection
```

## Overview

An `AnyRandomAccessCollection` instance forwards its operations to a base collection having the same `Element` type, hiding the specifics of the underlying collection.

## Topics

### Initializers

init&lt;C>(C)

Creates a type-erased collection that wraps the given collection.

init?(AnyBidirectionalCollection&lt;Element>)

Creates an `AnyRandomAccessCollection` having the same underlying collection as `other`.

init(AnyRandomAccessCollection&lt;Element>)

Creates an `AnyRandomAccessCollection` having the same underlying collection as `other`.

init?(AnyCollection&lt;Element>)

Creates an `AnyRandomAccessCollection` having the same underlying collection as `other`.

### Instance Methods

func drop(while: (Element) throws -> Bool) rethrows -> AnyRandomAccessCollection&lt;Element>

func dropFirst(Int) -> AnyRandomAccessCollection&lt;Element>

func dropLast(Int) -> AnyRandomAccessCollection&lt;Element>

func filter((Element) throws -> Bool) rethrows -> [Element]

func forEach((Element) throws -> Void) rethrows

func formIndex(inout AnyRandomAccessCollection&lt;Element>.Index, offsetBy: Int)

func formIndex(inout AnyRandomAccessCollection&lt;Element>.Index, offsetBy: Int, limitedBy: AnyRandomAccessCollection&lt;Element>.Index) -> Bool

func map&lt;T, E>((Element) throws(E) -> T) throws(E) -> [T]

func prefix(Int) -> AnyRandomAccessCollection&lt;Element>

func prefix(while: (Element) throws -> Bool) rethrows -> AnyRandomAccessCollection&lt;Element>

func suffix(Int) -> AnyRandomAccessCollection&lt;Element>

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Collection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- RandomAccessCollection

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

struct AnyIterator

A type-erased iterator of `Element`.

struct AnyIndex

A wrapper over an underlying index that hides the specific underlying type.

struct AnyHashable

A type-erased hashable value.

