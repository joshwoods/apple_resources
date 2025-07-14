

- Swift
- ClosedRange
-  ClosedRange.Index 

Enumeration

# ClosedRange.Index

A type that represents a position in the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum Index
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## Overview

Valid indices consist of the position of every element and a “past the end” position that’s not valid for use as a subscript argument.

## Topics

### Enumeration Cases

case inRange(Bound)

case pastEnd

### Default Implementations

Comparable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Comparable

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- Copyable

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- Equatable

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- Hashable

  Conforms when `Bound` conforms to `Hashable`, `Bound` conforms to `Strideable`, and `Bound.Stride` conforms to `SignedInteger`.

- Sendable

  Conforms when `Bound` conforms to `Sendable`, `Bound` conforms to `Strideable`, and `Bound.Stride` conforms to `SignedInteger`.

