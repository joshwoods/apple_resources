

- Swift
- Swift Standard Library
- Manual Memory Management
- UnsafeRawPointer
-  AtomicOptionalRepresentable Implementations 

API Collection

# AtomicOptionalRepresentable Implementations

## Topics

### Type Aliases

typealias AtomicOptionalRepresentation

The storage representation type that encodes to and decodes from `Optional` which is a suitable type when used in atomic operations on `Optional`.

### Type Methods

static func decodeAtomicOptionalRepresentation(consuming UnsafeRawPointer.AtomicOptionalRepresentation) -> UnsafeRawPointer?

Recovers the logical atomic type `Self?` by destroying some `AtomicOptionalRepresentation` storage instance returned from an atomic operation on `Optional`.

static func encodeAtomicOptionalRepresentation(consuming UnsafeRawPointer?) -> UnsafeRawPointer.AtomicOptionalRepresentation

Destroys a value of `Self` and prepares an `AtomicOptionalRepresentation` storage type to be used for atomic operations on `Optional`.

