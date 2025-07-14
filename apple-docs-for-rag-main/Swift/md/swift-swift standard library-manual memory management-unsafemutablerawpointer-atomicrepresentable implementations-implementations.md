

- Swift
- Swift Standard Library
- Manual Memory Management
- UnsafeMutableRawPointer
-  AtomicRepresentable Implementations 

API Collection

# AtomicRepresentable Implementations

## Topics

### Type Aliases

typealias AtomicRepresentation

The storage representation type that `Self` encodes to and decodes from which is a suitable type when used in atomic operations.

### Type Methods

static func decodeAtomicRepresentation(consuming UnsafeMutableRawPointer.AtomicRepresentation) -> UnsafeMutableRawPointer

Recovers the logical atomic type `Self` by destroying some `AtomicRepresentation` storage instance returned from an atomic operation.

static func encodeAtomicRepresentation(consuming UnsafeMutableRawPointer) -> UnsafeMutableRawPointer.AtomicRepresentation

Destroys a value of `Self` and prepares an `AtomicRepresentation` storage type to be used for atomic operations.

