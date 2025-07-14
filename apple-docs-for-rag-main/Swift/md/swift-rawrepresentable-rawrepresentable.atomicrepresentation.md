

- Swift
- RawRepresentable
-  RawRepresentable.AtomicRepresentation 

Type Alias

# RawRepresentable.AtomicRepresentation

The storage representation type that `Self` encodes to and decodes from which is a suitable type when used in atomic operations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
typealias AtomicRepresentation = Self.RawValue.AtomicRepresentation
```

Available when `Self` conforms to `AtomicRepresentable` and `RawValue` conforms to `AtomicRepresentable`.

