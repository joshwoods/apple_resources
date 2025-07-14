

- CloudKit
- CKOperation
-  operationID 

Instance Property

# operationID

A unique identifier for a long-lived operation.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.12+tvOS 9.2+visionOSwatchOS 3.0+Swift 4.2+

``` source
var operationID: CKOperation.ID { get }
```

## Discussion

Pass this property’s value to the fetchLongLivedOperationWithID:completionHandler: method to fetch the corresponding long-lived operation. For more information, see Long-Lived Operations.

## See Also

### Identifying the Operation

typealias ID

A type that represents the ID of an operation.

