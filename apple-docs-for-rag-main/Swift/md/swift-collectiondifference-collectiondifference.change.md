

- Swift
- CollectionDifference
-  CollectionDifference.Change 

Enumeration

# CollectionDifference.Change

A single change to a collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
enum Change
```

## Topics

### Enumeration Cases

case insert(offset: Int, element: ChangeElement, associatedWith: Int?)

An insertion.

case remove(offset: Int, element: ChangeElement, associatedWith: Int?)

A removal.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `ChangeElement` conforms to `Equatable`.

- Decodable

  Conforms when `ChangeElement` conforms to `Decodable` and `Encodable`.

- Encodable

  Conforms when `ChangeElement` conforms to `Decodable` and `Encodable`.

- Equatable

  Conforms when `ChangeElement` conforms to `Equatable`.

- Hashable

  Conforms when `ChangeElement` conforms to `Hashable`.

- Sendable

  Conforms when `ChangeElement` conforms to `Copyable`, `Escapable`, and `Sendable`.

