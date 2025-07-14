

- Core Data
-  NSPersistentCloudKitContainer 

Class

# NSPersistentCloudKitContainer

A container that encapsulates the Core Data stack in your app, and mirrors select persistent stores to a CloudKit private database.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NSPersistentCloudKitContainer
```

## Mentioned in 

Setting Up Core Data with CloudKit

Reading CloudKit Records for Core Data

Mirroring a Core Data store with CloudKit

## Overview

NSPersistentCloudKitContainer is a subclass of NSPersistentContainer capable of managing both CloudKit-backed and noncloud stores.

By default, NSPersistentCloudKitContainer contains a single store description, which Core Data assigns to the first CloudKit container identifier in an app’s entitlements. Use NSPersistentCloudKitContainerOptions to customize this behavior or create additional store descriptions with backing by different containers.

For more information about setting up multiple stores, see Setting Up Core Data with CloudKit.

## Topics

### Checking Permissions

func canUpdateRecord(forManagedObjectWith: NSManagedObjectID) -> Bool

Returns a Boolean value that indicates whether the user can modify the managed object’s underlying CloudKit record.

func canDeleteRecord(forManagedObjectWith: NSManagedObjectID) -> Bool

Returns a Boolean value that indicates whether the user can delete the managed object’s underlying CloudKit record.

func canModifyManagedObjects(in: NSPersistentStore) -> Bool

Returns a Boolean value that indicates whether the user can modify the specified persistent store.

### Sharing Objects

Accepting Share Invitations in a SwiftUI App

Adapt your app to use UIKit’s application and scene delegates so it can process CloudKit share invitations.

### Promoting Your Schema

func initializeCloudKitSchema(options: NSPersistentCloudKitContainerSchemaInitializationOptions) throws

Creates the CloudKit schema for all stores in the container that manage a CloudKit database.

struct NSPersistentCloudKitContainerSchemaInitializationOptions

Options that control the behavior when promoting the container’s schema to CloudKit.

### Monitoring Container Events

class Event

An object that represents activity in a persistent CloudKit container.

enum EventType

The type of event in a persistent CloudKit container, either setup, import, or export.

class NSPersistentCloudKitContainerEventRequest

A request to fetch setup, import, or export events in a persistent CloudKit container.

class NSPersistentCloudKitContainerEventResult

The result of a request to fetch persistent CloudKit container events.

class let eventChangedNotification: NSNotification.Name

A notification that contains details about an event in a persistent CloudKit container.

class let eventNotificationUserInfoKey: String

The user info dictionary key for the persistent CloudKit container event.

## Relationships

### Inherits From

- NSPersistentContainer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### CloudKit mirroring

Mirroring a Core Data store with CloudKit

Back user interfaces with a local replica of a CloudKit private database.

Synchronizing a local store to the cloud

Share data between a user’s devices and other iCloud users.

class NSPersistentCloudKitContainerOptions

An object that customizes how a store description aligns with a CloudKit database.

Sharing Core Data objects between iCloud users

Use Core Data and CloudKit to synchronize data between devices of an iCloud user and share data between different iCloud users.

