

- CloudKit
-  CKOperationGroup 

Class

# CKOperationGroup

An explicit association between two or more operations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class CKOperationGroup
```

## Overview

In certain situations, you might want to perform several CloudKit operations together. Grouping operations in CloudKit doesn’t ensure atomicity.

For example, when building a Calendar app, you group the following actions:

- Fetch records from CloudKit, which consists of numerous queries that fetch both new records and records with changes.

- Perform incremental fetches of records in response to a push notification.

- Update several records when the user saves a calendar event.

Associate operation groups with operations by setting their group property. Create a new operation group for each distinct user interaction.

## Topics

### Creating an Operation Group

init()

Creates an operation group.

init(coder: NSCoder)

Creates an operation group from a serialized instance.

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

enum TransferSize

Constants that represent possible data transfer sizes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Core objects

class CKContainer

A conduit to your app’s databases.

class CKDatabase

An object that represents a collection of record zones and subscriptions.

