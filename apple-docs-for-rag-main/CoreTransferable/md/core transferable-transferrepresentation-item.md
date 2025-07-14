

- Core Transferable
- TransferRepresentation
-  Item 

Associated Type

# Item

The type of the item that’s being transferred.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
associatedtype Item : Transferable
```

**Required**

## See Also

### Implementing a transfer representation

var body: Self.Body

A builder expression that describes the process of importing and exporting an item.

**Required**

associatedtype Body : TransferRepresentation

The transfer representation for the item.

**Required**

