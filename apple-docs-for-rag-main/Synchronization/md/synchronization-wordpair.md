

- Synchronization
-  WordPair 

Structure

# WordPair

A pair of two word sized `UInt`s.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct WordPair
```

## Overview

This type’s primary purpose is to be used in double wide atomic operations. On platforms that support it, atomic operations on `WordPair` are done in a single operation for two words. Users can use this type as itself when used on `Atomic`, or it could be used as an intermediate step for custom `AtomicRepresentable` types that are also double wide.

```
let atomicPair = Atomic(WordPair(first: 0, second: 0))
atomicPair.store(WordPair(first: someVersion, second: .max), ordering: .relaxed)
```

When used as an intermediate step for custom `AtomicRepresentable` types, it is critical that their `AtomicRepresentation` be equal to `WordPair.AtomicRepresentation`.

```
struct GridPoint {
  var x: Int
  var y: Int
}

extension GridPoint: AtomicRepresentable {
  typealias AtomicRepresentation = WordPair.AtomicRepresentation

  ...
}
```

Note

This type only conforms to `AtomicRepresentable` on platforms that support double wide atomics.

## Topics

### Initializers

init(first: UInt, second: UInt)

Initialize a new `WordPair` value given both individual words.

### Instance Properties

var first: UInt

The first element in this word pair.

var second: UInt

The second element in this word pair.

### Default Implementations

AtomicRepresentable Implementations

Comparable Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- AtomicRepresentable
- BitwiseCopyable
- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Atomic Values

struct Atomic

An atomic value.

struct AtomicLazyReference

A lazily initializable atomic strong reference.

protocol AtomicRepresentable

A type that supports atomic operations through a separate atomic storage representation.

protocol AtomicOptionalRepresentable

An atomic value that also supports atomic operations when wrapped in an `Optional`. Atomic optional representable types come with a standalone atomic representation for their optional-wrapped variants.

