

- Core Transferable
- TransferRepresentation
-  body 

Instance Property

# body

A builder expression that describes the process of importing and exporting an item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@TransferRepresentationBuilder var body: Self.Body { get }
```

**Required**

## Discussion

Combine multiple existing transfer representations to compose a single transfer representation that describes how to transfer an item in multiple scenarios.

```
struct CombinedRepresentation: TransferRepresentation {
   var body: some TransferRepresentation {
       DataRepresentation(...)
       FileRepresentation(...)
   }
}
```

## See Also

### Implementing a transfer representation

associatedtype Body : TransferRepresentation

The transfer representation for the item.

**Required**

associatedtype Item : Transferable

The type of the item that’s being transferred.

**Required**

