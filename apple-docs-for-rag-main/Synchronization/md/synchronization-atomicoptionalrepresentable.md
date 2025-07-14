

- Synchronization
-  AtomicOptionalRepresentable 

Protocol

# AtomicOptionalRepresentable

An atomic value that also supports atomic operations when wrapped in an `Optional`. Atomic optional representable types come with a standalone atomic representation for their optional-wrapped variants.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol AtomicOptionalRepresentable : AtomicRepresentable
```

## Topics

### Associated Types

associatedtype AtomicOptionalRepresentation : BitwiseCopyable

The storage representation type that encodes to and decodes from `Optional` which is a suitable type when used in atomic operations on `Optional`.

**Required**

### Type Methods

static func decodeAtomicOptionalRepresentation(consuming Self.AtomicOptionalRepresentation) -> Self?

Recovers the logical atomic type `Self?` by destroying some `AtomicOptionalRepresentation` storage instance returned from an atomic operation on `Optional`.

**Required**

static func encodeAtomicOptionalRepresentation(consuming Self?) -> Self.AtomicOptionalRepresentation

Destroys a value of `Self` and prepares an `AtomicOptionalRepresentation` storage type to be used for atomic operations on `Optional`.

**Required**

## Relationships

### Inherits From

- AtomicRepresentable

### Conforming Types

- ObjectIdentifier
- OpaquePointer
- Unmanaged

  Conforms when `Instance` conforms to `Copyable` and `Escapable`.

- UnsafeMutablePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeMutableRawPointer
- UnsafePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeRawPointer

## See Also

### Atomic Values

struct Atomic

An atomic value.

struct AtomicLazyReference

A lazily initializable atomic strong reference.

struct WordPair

A pair of two word sized `UInt`s.

protocol AtomicRepresentable

A type that supports atomic operations through a separate atomic storage representation.

