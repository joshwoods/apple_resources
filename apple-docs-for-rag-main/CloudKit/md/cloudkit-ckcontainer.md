

- CloudKit
-  CKContainer 

Class

# CKContainer

A conduit to your app’s databases.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKContainer
```

## Mentioned in 

Identifying an App’s Containers

Designing and Creating a CloudKit Database

## Overview

A container manages all explicit and implicit attempts to access its contents.

Every app has a default container that manages its own content. If you develop a suite of apps, you can access any containers that you have the appropriate entitlements for. Each new container distinguishes between public and private data. CloudKit always stores private data in the appropriate container directory in the user’s iCloud account.

Note

`CKContainer` instances operate with a QualityOfService.userInitiated quality of service level by default. For information about quality of service, see Prioritize Work with Quality of Service Classes in Energy Efficiency Guide for iOS Apps and Prioritize Work at the Task Level in Energy Efficiency Guide for Mac Apps.

### Interacting with a Container

A container coordinates all interactions between your app and the server. Most of these interactions involve the following tasks:

- Determining whether the user has an iCloud account, which lets you know if you can write data to the user’s personal storage.

- With the user’s permission, discovering other users who the current user knows, and making the current user’s information discoverable.

- Getting the container or one of its databases to use with an operation.

### Public and Private Databases

Each container provides a public and a private database for storing data. The contents of the public database are accessible to all users of the app, whereas the contents of the private database are, by default, visible only to the current user. Content that is specific to a single user usually belongs in that user’s private database, whereas app-related content that you provide (or that users want to share) belongs in the public database.

The public database is always available, regardless of whether the device has an active iCloud account. When there isn’t an iCloud account, your app can fetch records from and query the public database, but it can’t save changes. Saving records to the public database requires an active iCloud account to identify the owner of those records. Access to the private database always requires an active iCloud account on the device.

Note

The data in a public database counts toward the iCloud storage quota of the app that owns the container. That data doesn’t count toward the storage quota of any single user. Data in the private database counts toward the user’s iCloud storage quota.

### Using iCloud

Whenever possible, design your app to run gracefully with or without an active iCloud account. Even without an active iCloud account, apps can fetch records from the public database and display that information to the user. If your app requires the ability to write to the public database or requires access to the private database, notify the user of the reason and encourage them to enable iCloud. You can even provide a button that takes the user directly to Settings so that they can enable iCloud. To implement such a button, have the button’s action open the URL that the openSettingsURLString constant provides.

### User Records and Permissions

When a user accesses a container for the first time, CloudKit assigns them a unique identifier and uses it to create two user records — one in the app’s public database and another in that user’s private database. By default, these records don’t contain any identifying personal information, but you can use the record in the user’s private database to store additional, nonsensitive information about that user. Because the public database’s user record is accessible to all users of your app, don’t use it to store information about the user.

While a user record isn’t the same as the user’s CKUserIdentity, the identity does provide the identifier of their user record that you can use to fetch that record from either the public database or the user’s private database. For more information, see userRecordID.

### Testing Your Code Using the Development Container

At runtime, CloudKit uses your app’s `com.apple.developer.icloud-container-environment` entitlement to discover whether you’re using a `Development` or `Production` version of your provisioning profile. When you configure the entitlement for development, CloudKit configures the app’s containers to use the development server. The development environment is a safe place to make changes during the development process without disrupting users of your app. You can add new fields to records programmatically, and you can delete or modify fields using iCloud Dashboard.

Before shipping your app, always test your app’s behavior in the production environment. The production server generates errors when your app tries to add record types or add new fields to existing record types. Testing in the production environment helps you find and fix the places in your code where you’re making those types of changes. You can use CloudKit Dashboard to modify record types in the development environment, and then migrate those changes to the production environment.

Note

Simulator works only with the development environment. When you’re ready to test your app in a production environment, do so from a device.

## Topics

### Creating Containers

class func `default`() -> CKContainer

Returns the app’s default container.

init(identifier: String)

Creates a container for the specified identifier.

### Getting the Public and Private Databases

var privateCloudDatabase: CKDatabase

The user’s private database.

var publicCloudDatabase: CKDatabase

The app’s public database.

var sharedCloudDatabase: CKDatabase

The database that contains shared data.

func database(with: CKDatabase.Scope) -> CKDatabase

Returns the database with the specified scope.

### Getting the Container’s Identifier

var containerIdentifier: String?

The container’s unique identifier.

### Determining the User’s iCloud Access Status

func accountStatus(completionHandler: (CKAccountStatus, (any Error)?) -> Void)

Determines whether the system can access the user’s iCloud account.

enum CKAccountStatus

Constants that indicate the availability of the user’s iCloud account.

### Requesting and Determining App Permissions

func requestApplicationPermission(CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Prompts the user to authorize the specified permission.

Deprecated

func status(forApplicationPermission: CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Determines the authorization status of the specified permission.

Deprecated

enum Application

A collection of types for app permissions.

struct ApplicationPermissions

Constants that represent the permissions that a user grants.

typealias ApplicationPermissionBlock

A closure that processes the outcome of a permissions request.

Deprecated

enum ApplicationPermissionStatus

Constants that represent the status of a permission.

Deprecated

### Performing Operations on the Container

func add(CKOperation)

Adds an operation to the container’s queue.

### Discovering User Records

func discoverAllIdentities(completionHandler: ([CKUserIdentity]?, (any Error)?) -> Void)

Fetches all user identities that match entries in the user’s Contacts.

Deprecated

func discoverUserIdentity(withEmailAddress: String, completionHandler: (CKUserIdentity?, (any Error)?) -> Void)

Fetches the user identity for the specified email address.

Deprecated

func discoverUserIdentity(withPhoneNumber: String, completionHandler: (CKUserIdentity?, (any Error)?) -> Void)

Fetches the user identity for the specified phone number.

Deprecated

func discoverUserIdentity(withUserRecordID: CKRecord.ID, completionHandler: (CKUserIdentity?, (any Error)?) -> Void)

Fetches the user identity for the specified user record ID.

Deprecated

func fetchShareParticipant(withEmailAddress: String, completionHandler: (CKShare.Participant?, (any Error)?) -> Void)

Fetches the share participant with the specified email address.

func fetchShareParticipant(withPhoneNumber: String, completionHandler: (CKShare.Participant?, (any Error)?) -> Void)

Fetches the share participant with the specified phone number.

func fetchShareParticipant(withUserRecordID: CKRecord.ID, completionHandler: (CKShare.Participant?, (any Error)?) -> Void)

Fetches the share participant with the specified user record ID.

func fetchUserRecordID(completionHandler: (CKRecord.ID?, (any Error)?) -> Void)

Fetches the user record ID of the current user.

let CKCurrentUserDefaultName: String

A constant that provides the current user’s default name.

let CKOwnerDefaultName: String

A constant that provides the default owner’s name.

Deprecated

### Fetching Long-Lived Operations

func fetchAllLongLivedOperationIDs(completionHandler: ([CKOperation.ID]?, (any Error)?) -> Void)

Fetches the IDs of any long-lived operations that are running.

func fetchLongLivedOperation(withID: CKOperation.ID, completionHandler: (CKOperation?, (any Error)?) -> Void)

Fetches the long-lived operation for the specified operation ID.

### Accessing Container Metadata

func fetchShareMetadata(with: URL, completionHandler: (CKShare.Metadata?, (any Error)?) -> Void)

Fetches the share metadata for the specified share URL.

func accept(CKShare.Metadata, completionHandler: (CKShare?, (any Error)?) -> Void)

Accepts the specified share metadata.

static let CKAccountChanged: NSNotification.Name

A notification that a container posts when the status of an iCloud account changes.

### Instance Methods

func accept([CKShare.Metadata]) async throws -> [CKShare.Metadata : Result&lt;CKShare, any Error>]

func accept([CKShare.Metadata], completionHandler: (Result&lt;[CKShare.Metadata : Result&lt;CKShare, any Error>], any Error>) -> Void)

func allLongLivedOperationIDs() async throws -> [CKOperation.ID]

func configuredWith&lt;R>(configuration: CKOperation.Configuration?, group: CKOperationGroup?, body: (CKContainer) throws -> R) rethrows -> R

func configuredWith&lt;R>(configuration: CKOperation.Configuration?, group: CKOperationGroup?, body: (CKContainer) async throws -> R) async rethrows -> R

func discoverUserIdentities(forEmailAddresses: [String], completionHandler: (Result&lt;[String : CKUserIdentity], any Error>) -> Void)Deprecated

func discoverUserIdentities(forPhoneNumbers: [String], completionHandler: (Result&lt;[String : CKUserIdentity], any Error>) -> Void)Deprecated

func discoverUserIdentities(forUserRecordIDs: [CKRecord.ID], completionHandler: (Result&lt;[CKRecord.ID : CKUserIdentity], any Error>) -> Void)Deprecated

func fetchShareMetadatas(for: [URL], completionHandler: (Result&lt;[URL : Result&lt;CKShare.Metadata, any Error>], any Error>) -> Void)

func fetchShareParticipants(forEmailAddresses: [String], completionHandler: (Result&lt;[String : Result&lt;CKShare.Participant, any Error>], any Error>) -> Void)

func fetchShareParticipants(forPhoneNumbers: [String], completionHandler: (Result&lt;[String : Result&lt;CKShare.Participant, any Error>], any Error>) -> Void)

func fetchShareParticipants(forUserRecordIDs: [CKRecord.ID], completionHandler: (Result&lt;[CKRecord.ID : Result&lt;CKShare.Participant, any Error>], any Error>) -> Void)

func longLivedOperation(for: CKOperation.ID) async throws -> CKOperation?

func shareMetadatas(for: [URL]) async throws -> [URL : Result&lt;CKShare.Metadata, any Error>]

func shareParticipants(forEmailAddresses: [String]) async throws -> [String : Result&lt;CKShare.Participant, any Error>]

func shareParticipants(forPhoneNumbers: [String]) async throws -> [String : Result&lt;CKShare.Participant, any Error>]

func shareParticipants(forUserRecordIDs: [CKRecord.ID]) async throws -> [CKRecord.ID : Result&lt;CKShare.Participant, any Error>]

func userIdentities(forEmailAddresses: [String]) async throws -> [String : CKUserIdentity]Deprecated

func userIdentities(forPhoneNumbers: [String]) async throws -> [String : CKUserIdentity]Deprecated

func userIdentities(forUserRecordIDs: [CKRecord.ID]) async throws -> [CKRecord.ID : CKUserIdentity]Deprecated

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
- Sendable

## See Also

### Core objects

class CKDatabase

An object that represents a collection of record zones and subscriptions.

class CKOperationGroup

An explicit association between two or more operations.

