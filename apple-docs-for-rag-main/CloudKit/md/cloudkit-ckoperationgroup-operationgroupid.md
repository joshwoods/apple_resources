

- CloudKit
- CKOperationGroup
-  operationGroupID 

Instance Property

# operationGroupID

The operation group’s unique identifier.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var operationGroupID: String { get }
```

## Discussion

The framework generates this value and it’s unique to this operation group. The system sends this identifier to CloudKit, which can use it to identify server-side logs for CKOperationGroup.

## See Also

### Configuring an Operation Group

var defaultConfiguration: CKOperation.Configuration!

The default configuration for operations in the group.

var expectedReceiveSize: CKOperationGroup.TransferSize

The estimated size of traffic to download from CloudKit.

var expectedSendSize: CKOperationGroup.TransferSize

The estimated size of traffic to upload to CloudKit.

var name: String?

The operation group’s name.

var quantity: Int

The number of operations in the operation group.

enum TransferSize

Constants that represent possible data transfer sizes.

