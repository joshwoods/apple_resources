

- CloudKit
- CKOperationGroup
-  defaultConfiguration 

Instance Property

# defaultConfiguration

The default configuration for operations in the group.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@NSCopying
var defaultConfiguration: CKOperation.Configuration! { get set }
```

## Discussion

If an operation in the group has its own configuration, that configuration’s values override the default configuration’s values. For more information, see CKOperation.Configuration.

## See Also

### Configuring an Operation Group

var expectedReceiveSize: CKOperationGroup.TransferSize

The estimated size of traffic to download from CloudKit.

var expectedSendSize: CKOperationGroup.TransferSize

The estimated size of traffic to upload to CloudKit.

var name: String?

The operation group’s name.

var operationGroupID: String

The operation group’s unique identifier.

var quantity: Int

The number of operations in the operation group.

enum TransferSize

Constants that represent possible data transfer sizes.

