

- Swift
-  Hasher 

Structure

# Hasher

The universal hash function used by `Set` and `Dictionary`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Hasher
```

## Overview

`Hasher` can be used to map an arbitrary sequence of bytes to an integer hash value. You can feed data to the hasher using a series of calls to mutating `combine` methods. When you’ve finished feeding the hasher, the hash value can be retrieved by calling `finalize()`:

```
var hasher = Hasher()
hasher.combine(23)
hasher.combine("Hello")
let hashValue = hasher.finalize()
```

Within the execution of a Swift program, `Hasher` guarantees that finalizing it will always produce the same hash value as long as it is fed the exact same sequence of bytes. However, the underlying hash algorithm is designed to exhibit avalanche effects: slight changes to the seed or the input byte sequence will typically produce drastic changes in the generated hash value.

Note

Do not save or otherwise reuse hash values across executions of your program. `Hasher` is usually randomly seeded, which means it will return different values on every new execution of your program. The hash algorithm implemented by `Hasher` may itself change between any two versions of the standard library.

## Topics

### Creating a Hasher

init()

Creates a new hasher.

### Adding Values

func combine&lt;H>(H)

Adds the given value to this hasher, mixing its essential parts into the hasher state.

func combine(bytes: UnsafeRawBufferPointer)

Adds the contents of the given buffer to this hasher, mixing it into the hasher state.

### Finalizing a Hasher

func finalize() -> Int

Finalizes the hasher state and returns the hash value.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

## See Also

### Sets and Dictionaries

protocol Hashable

A type that can be hashed into a `Hasher` to produce an integer hash value.

