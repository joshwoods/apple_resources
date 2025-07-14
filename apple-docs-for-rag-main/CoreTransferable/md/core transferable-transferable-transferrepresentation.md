

- Core Transferable
- Transferable
-  transferRepresentation 

Type Property

# transferRepresentation

The representation used to import and export the item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@TransferRepresentationBuilder static var transferRepresentation: Self.Representation { get }
```

**Required**

## Mentioned in 

Choosing a transfer representation for a model type

## Discussion

A transferRepresentation can contain multiple representations for different content types.

## See Also

### Implementing a transfer representation

associatedtype Representation : TransferRepresentation

The type of the representation used to import and export the item.

**Required**

