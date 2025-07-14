

- CloudKit
- CKOperationGroup
-  name 

Instance Property

# name

The operation group’s name.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var name: String? { get set }
```

## Discussion

The system sends the name of the operation group to CloudKit to provide aggregate reporting for CKOperationGroup. The name must not include any personal data.

## See Also

### Configuring an Operation Group

var defaultConfiguration: CKOperation.Configuration!

The default configuration for operations in the group.

var expectedReceiveSize: CKOperationGroup.TransferSize

The estimated size of traffic to download from CloudKit.

var expectedSendSize: CKOperationGroup.TransferSize

The estimated size of traffic to upload to CloudKit.

var operationGroupID: String

The operation group’s unique identifier.

var quantity: Int

The number of operations in the operation group.

enum TransferSize

Constants that represent possible data transfer sizes.

