

- Swift
- LazyPrefixWhileSequence
-  LazyPrefixWhileSequence.Iterator 

Structure

# LazyPrefixWhileSequence.Iterator

An iterator over the initial elements traversed by a base iterator that satisfy a given predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Base` conforms to `Sequence`.

## Overview

This is the associated iterator for the `LazyPrefixWhileSequence`, `LazyPrefixWhileCollection`, and `LazyPrefixWhileBidirectionalCollection` types.

## Topics

### Type Aliases

typealias Element

The type of element traversed by the iterator.

### Default Implementations

IteratorProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Base` conforms to `Sequence`.

- IteratorProtocol

  Conforms when `Base` conforms to `Sequence`.

- Sequence

  Conforms when `Base` conforms to `Sequence`.

