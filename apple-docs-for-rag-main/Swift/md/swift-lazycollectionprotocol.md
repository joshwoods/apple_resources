

- Swift
-  LazyCollectionProtocol 

Protocol

# LazyCollectionProtocol

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol LazyCollectionProtocol : Collection, LazySequenceProtocol where Self.Elements : Collection
```

## Topics

### Instance Properties

var lazy: Self.Elements

var lazy: LazyCollection&lt;Self.Elements>

## Relationships

### Inherits From

- Collection
- LazySequenceProtocol
- Sequence

### Conforming Types

- LazyDropWhileSequence

  Conforms when `Base` conforms to `Collection`.

- LazyFilterSequence

  Conforms when `Base` conforms to `Collection`.

- LazyMapSequence

  Conforms when `Base` conforms to `Collection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazyPrefixWhileSequence

  Conforms when `Base` conforms to `Collection`.

- LazySequence

  Conforms when `Base` conforms to `Collection`.

## See Also

### Lazy Collections

protocol LazySequenceProtocol

A sequence on which normally-eager sequence operations are implemented lazily.

