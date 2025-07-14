

- Swift
- Swift Standard Library
- C Interoperability
- OpaquePointer
-  AtomicOptionalRepresentable Implementations 

API Collection

# AtomicOptionalRepresentable Implementations

## Topics

### Type Aliases

typealias AtomicOptionalRepresentation

The storage representation type that encodes to and decodes from `Optional` which is a suitable type when used in atomic operations on `Optional`.

### Type Methods

static func decodeAtomicOptionalRepresentation(consuming OpaquePointer.AtomicOptionalRepresentation) -> OpaquePointer?

Recovers the logical atomic type `Self?` by destroying some `AtomicOptionalRepresentation` storage instance returned from an atomic operation on `Optional`.

static func encodeAtomicOptionalRepresentation(consuming OpaquePointer?) -> OpaquePointer.AtomicOptionalRepresentation

Destroys a value of `Self` and prepares an `AtomicOptionalRepresentation` storage type to be used for atomic operations on `Optional`.

