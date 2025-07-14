

- Swift
- CollectionOfOne
-  CollectionOfOne.Iterator 

Structure

# CollectionOfOne.Iterator

An iterator that produces one or zero instances of an element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

## Overview

`IteratorOverOne` is the iterator for the `CollectionOfOne` type.

## Topics

### Default Implementations

IteratorProtocol Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- IteratorProtocol

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sendable

  Conforms when `Element` conforms to `Copyable`, `Escapable`, and `Sendable`.

