

- Swift
- Swift Standard Library
- Manual Memory Management
- Unmanaged
-  AtomicRepresentable Implementations 

API Collection

# AtomicRepresentable Implementations

## Topics

### Type Aliases

typealias AtomicRepresentation

The storage representation type that `Self` encodes to and decodes from which is a suitable type when used in atomic operations.

### Type Methods

static func decodeAtomicRepresentation(consuming Unmanaged&lt;Instance>.AtomicRepresentation) -> Unmanaged&lt;Instance>

Recovers the logical atomic type `Self` by destroying some `AtomicRepresentation` storage instance returned from an atomic operation.

static func encodeAtomicRepresentation(consuming Unmanaged&lt;Instance>) -> Unmanaged&lt;Instance>.AtomicRepresentation

Destroys a value of `Self` and prepares an `AtomicRepresentation` storage type to be used for atomic operations.

