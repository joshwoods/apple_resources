

- Core Transferable
-  TupleTransferRepresentation 

Structure

# TupleTransferRepresentation

A wrapper type for tuples that contain transfer representations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct TupleTransferRepresentation where Item : Transferable, Value : Sendable
```

## Topics

### Building a transfer representation

var body: some TransferRepresentation

A builder expression that describes the process of importing and exporting an item.

### Type Aliases

typealias Body

The transfer representation for the item.

### Default Implementations

TransferRepresentation Implementations

## Relationships

### Conforms To

- Sendable
- TransferRepresentation

## See Also

### Supporting types

struct TransferRepresentationBuilder

Creates a transfer representation by composing existing transfer representations.

