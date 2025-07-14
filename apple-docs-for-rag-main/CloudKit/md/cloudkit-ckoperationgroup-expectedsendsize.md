

- CloudKit
- CKOperationGroup
-  expectedSendSize 

Instance Property

# expectedSendSize

The estimated size of traffic to upload to CloudKit.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var expectedSendSize: CKOperationGroup.TransferSize { get set }
```

## Discussion

This property informs the system about the amount of data your app can transfer. An order-of-magnitude estimate is better than no estimate, and accuracy helps performance. The system checks this value when it schedules discretionary network requests.

## See Also

### Configuring an Operation Group

var defaultConfiguration: CKOperation.Configuration!

The default configuration for operations in the group.

var expectedReceiveSize: CKOperationGroup.TransferSize

The estimated size of traffic to download from CloudKit.

var name: String?

The operation group’s name.

var operationGroupID: String

The operation group’s unique identifier.

var quantity: Int

The number of operations in the operation group.

enum TransferSize

Constants that represent possible data transfer sizes.

