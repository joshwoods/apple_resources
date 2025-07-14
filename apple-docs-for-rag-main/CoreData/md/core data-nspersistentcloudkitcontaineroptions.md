

- Core Data
-  NSPersistentCloudKitContainerOptions 

Class

# NSPersistentCloudKitContainerOptions

An object that customizes how a store description aligns with a CloudKit database.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NSPersistentCloudKitContainerOptions
```

## Mentioned in 

Creating a Core Data Model for CloudKit

Setting Up Core Data with CloudKit

## Overview

Use NSPersistentCloudKitContainerOptions to customize the behavior of an NSPersistentCloudKitContainer or to create additional store descriptions that sync to other containers.

For more information about setting up multiple stores, see Setting Up Core Data with CloudKit.

## Topics

### Creating Container Options

init(containerIdentifier: String)

Initializes container options using the given CloudKit container identifier.

var containerIdentifier: String

The identifier of the CloudKit container associated with a given store description.

var databaseScope: CKDatabase.Scope

The database scope — public, private, or shared — to use for a specified store in a persistent CloudKit container.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### CloudKit mirroring

Mirroring a Core Data store with CloudKit

Back user interfaces with a local replica of a CloudKit private database.

Synchronizing a local store to the cloud

Share data between a user’s devices and other iCloud users.

class NSPersistentCloudKitContainer

A container that encapsulates the Core Data stack in your app, and mirrors select persistent stores to a CloudKit private database.

Sharing Core Data objects between iCloud users

Use Core Data and CloudKit to synchronize data between devices of an iCloud user and share data between different iCloud users.

