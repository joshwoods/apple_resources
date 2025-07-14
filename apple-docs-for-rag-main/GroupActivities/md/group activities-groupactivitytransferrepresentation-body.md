

- Group Activities
- GroupActivityTransferRepresentation
-  body 

Instance Property

# body

A builder expression that describes the process of importing and exporting an item.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

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

