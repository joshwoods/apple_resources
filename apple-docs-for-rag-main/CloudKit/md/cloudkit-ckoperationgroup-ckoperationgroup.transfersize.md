

- CloudKit
- CKOperationGroup
-  CKOperationGroup.TransferSize 

Enumeration

# CKOperationGroup.TransferSize

Constants that represent possible data transfer sizes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum TransferSize
```

## Topics

### Transfer Sizes

case kilobytes

A transfer size that represents 1 or more kilobytes.

case megabytes

A transfer size that represents 1 or more megabytes.

case gigabytes

A transfer size that represents 1 or more gigabytes.

case tensOfMegabytes

A transfer size that represents tens of megabytes.

case tensOfGigabytes

A transfer size that represents tens of gigabytes.

case hundredsOfMegabytes

A transfer size that represents hundreds of megabytes.

case hundredsOfGigabytes

A transfer size that represents hundreds of gigabytes.

case unknown

An unknown transfer size.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var quantity: Int

The number of operations in the operation group.

