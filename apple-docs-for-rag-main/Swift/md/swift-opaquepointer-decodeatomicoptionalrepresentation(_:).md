

- Swift
- OpaquePointer
-  decodeAtomicOptionalRepresentation(\_:) 

Type Method

# decodeAtomicOptionalRepresentation(\_:)

Recovers the logical atomic type `Self?` by destroying some `AtomicOptionalRepresentation` storage instance returned from an atomic operation on `Optional`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func decodeAtomicOptionalRepresentation(_ representation: consuming OpaquePointer.AtomicOptionalRepresentation) -> OpaquePointer?
```

## Return Value

The newly decoded logical type `Self?`.

## Discussion

Note

This is not an atomic operation. This simply decodes the storage representation used in atomic operations on `Optional` back into the logical type for normal use, `Self?`.

