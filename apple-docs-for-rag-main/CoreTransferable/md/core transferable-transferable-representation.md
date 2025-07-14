

- Core Transferable
- Transferable
-  Representation 

Associated Type

# Representation

The type of the representation used to import and export the item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
associatedtype Representation : TransferRepresentation
```

**Required**

## Discussion

Swift infers this type from the return value of the transferRepresentation property.

## See Also

### Implementing a transfer representation

static var transferRepresentation: Self.Representation

The representation used to import and export the item.

**Required**

