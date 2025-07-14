

- Vision
- BarcodeObservation
-  BarcodeObservation.CompositeType 

Enumeration

# BarcodeObservation.CompositeType

Composite types for barcode requests.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum CompositeType
```

## Topics

### Getting the composite types

case gs1TypeA

A type that represents trade items in bulk.

case gs1TypeB

A type that represents trade items by piece.

case gs1TypeC

A type that represents trade items in varying quantity.

case linked

A type that represents a linked composite type.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the composite type

let supplementalCompositeType: BarcodeObservation.CompositeType?

The supplemental composite type.

