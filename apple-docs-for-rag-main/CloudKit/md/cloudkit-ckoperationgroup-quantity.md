

- CloudKit
- CKOperationGroup
-  quantity 

Instance Property

# quantity

The number of operations in the operation group.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var quantity: Int { get set }
```

## Discussion

This property shows the number of operations that you expect to be in this operation group. It’s the developer’s responsibility to set this value.

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

var operationGroupID: String

The operation group’s unique identifier.

enum TransferSize

Constants that represent possible data transfer sizes.

