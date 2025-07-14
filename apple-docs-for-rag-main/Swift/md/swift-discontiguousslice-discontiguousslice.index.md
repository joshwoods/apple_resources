

- Swift
- DiscontiguousSlice
-  DiscontiguousSlice.Index 

Structure

# DiscontiguousSlice.Index

A position in a `DiscontiguousSlice`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Index
```

Available when `Base` conforms to `Collection`.

## Topics

### Instance Properties

let base: Base.Index

The position of this index in the base collection.

### Default Implementations

Comparable Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Comparable

  Conforms when `Base` conforms to `Collection`.

- Copyable

  Conforms when `Base` conforms to `Collection`.

- CustomStringConvertible

  Conforms when `Base` conforms to `Collection`.

- Equatable

  Conforms when `Base` conforms to `Collection`.

- Hashable

  Conforms when `Base` conforms to `Collection` and `Base.Index` conforms to `Hashable`.

- Sendable

  Conforms when `Base` conforms to `Collection` and `Base.Index` conforms to `Sendable`.

