

- Swift
-  DefaultIndices 

Structure

# DefaultIndices

A collection of indices for an arbitrary collection

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct DefaultIndices where Elements : Collection
```

## Topics

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Elements` conforms to `BidirectionalCollection`.

- Collection

  Conforms when `Elements` conforms to `RandomAccessCollection`.

- Copyable

  Conforms when `Elements` conforms to `Collection`.

- RandomAccessCollection

  Conforms when `Elements` conforms to `RandomAccessCollection`.

- Sendable

  Conforms when `Elements` conforms to `Collection`, `Elements` conforms to `Sendable`, and `Elements.Index` conforms to `Sendable`.

- Sequence

  Conforms when `Elements` conforms to `RandomAccessCollection`.

