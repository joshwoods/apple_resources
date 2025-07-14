

- Core Transferable
- TupleTransferRepresentation
-  body 

Instance Property

# body

A builder expression that describes the process of importing and exporting an item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var body: some TransferRepresentation { get }
```

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

