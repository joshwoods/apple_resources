

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- Int64
-  AtomicRepresentable Implementations 

API Collection

# AtomicRepresentable Implementations

## Topics

### Type Aliases

typealias AtomicRepresentation

The storage representation type that `Self` encodes to and decodes from which is a suitable type when used in atomic operations.

### Type Methods

static func decodeAtomicRepresentation(consuming Int64.AtomicRepresentation) -> Int64

Recovers the logical atomic type `Self` by destroying some `AtomicRepresentation` storage instance returned from an atomic operation.

static func encodeAtomicRepresentation(borrowing Int64) -> Int64.AtomicRepresentation

Destroys a value of `Self` and prepares an `AtomicRepresentation` storage type to be used for atomic operations.

