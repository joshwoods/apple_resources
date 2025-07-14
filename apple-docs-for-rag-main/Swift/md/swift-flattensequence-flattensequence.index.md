

- Swift
- FlattenSequence
-  FlattenSequence.Index 

Structure

# FlattenSequence.Index

A position in a FlattenCollection

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Index
```

Available when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

## Topics

### Default Implementations

Comparable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Comparable

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

- Copyable

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

- Equatable

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

- Hashable

  Conforms when `Base` conforms to `Collection`, `Base.Element` conforms to `Collection`, `Base.Index` conforms to `Hashable`, and `Base.Element.Index` conforms to `Hashable`.

- Sendable

  Conforms when `Base` conforms to `Collection`, `Base.Element` conforms to `Collection`, `Base.Index` conforms to `Sendable`, and `Base.Element.Index` conforms to `Sendable`.

