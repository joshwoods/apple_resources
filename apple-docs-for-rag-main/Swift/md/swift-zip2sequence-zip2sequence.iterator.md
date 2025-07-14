

- Swift
- Zip2Sequence
-  Zip2Sequence.Iterator 

Structure

# Zip2Sequence.Iterator

An iterator for `Zip2Sequence`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Sequence1` conforms to `Sequence` and `Sequence2` conforms to `Sequence`.

## Topics

### Default Implementations

IteratorProtocol Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Sequence1` conforms to `Sequence` and `Sequence2` conforms to `Sequence`.

- IteratorProtocol

  Conforms when `Sequence1` conforms to `Sequence` and `Sequence2` conforms to `Sequence`.

- Sendable

  Conforms when `Sequence1` conforms to `Sequence`, `Sequence2` conforms to `Sequence`, `Sequence1.Iterator` conforms to `Sendable`, and `Sequence2.Iterator` conforms to `Sendable`.

