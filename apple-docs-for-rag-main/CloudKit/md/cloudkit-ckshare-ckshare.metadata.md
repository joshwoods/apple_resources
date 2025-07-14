

- CloudKit
- CKShare
-  CKShare.Metadata 

Class

# CKShare.Metadata

An object that describes a shared record’s metadata.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class Metadata
```

## Overview

A share’s metadata is an intermediary object that provides access to the share, its owner, and, for a shared record hierarchy, its root record. Metadata also includes details about the current user’s participation in the share.

You don’t create metadata. CloudKit provides it to your app when the user taps or clicks a share’s url, such as in an email or a message. The method CloudKit calls varies by platform and app configuration, and includes the following:

- For a scene-based iOS app in a running or suspended state, CloudKit calls the windowScene(_:userDidAcceptCloudKitShareWith:) method on your window scene delegate.

- For a scene-based iOS app that’s not running, the system launches your app in response to the tap or click, and calls the scene(_:willConnectTo:options:) method on your scene delegate. The `connectionOptions` parameter contains the metadata. Use its cloudKitShareMetadata property to access it.

- For an iOS app that doesn’t use scenes, CloudKit calls your app delegate’s application(_:userDidAcceptCloudKitShareWith:) method.

- For a macOS app, CloudKit calls your app delegate’s application(_:userDidAcceptCloudKitShareWith:) method.

- For a watchOS app, CloudKit calls the userDidAcceptCloudKitShare(with:) method on your watch extension delegate.

Respond by checking the participantStatus of the provided metadata. If the status is `pending`, use CKAcceptSharesOperation to accept participation in the share. You can also fetch metadata independent of this flow using CKFetchShareMetadataOperation.

For a shared record hierarchy, the hierarchicalRootRecordID property contains the ID of the share’s root record. When using CKFetchShareMetadataOperation to fetch metadata, you can include the entire root record by setting the operation’s shouldFetchRootRecord property to true. CloudKit then populates the rootRecord property before it returns the metadata. You can further customize this behavior using the operation’s rootRecordDesiredKeys property to specify which fields to return. This functionality isn’t applicable for a shared record zone because, unlike a shared record hierarchy, it doesn’t have a nominated root record.

The participant properties provide the current user’s acceptance status, permissions, and role. Use these values to determine what functionality to provide to the user. For example, only display editing controls for accepted participants with `readWrite` permissions.

## Topics

### Accessing the Share

var share: CKShare

The share that owns the metadata.

var containerIdentifier: String

The ID of the share’s container.

var ownerIdentity: CKUserIdentity

The identity of the share’s owner.

### Accessing the Root Record

var hierarchicalRootRecordID: CKRecord.ID?

The record ID of the shared hierarchy’s root record.

var rootRecord: CKRecord?

The share’s root record.

var rootRecordID: CKRecord.ID

The record ID of the share’s root record.

Deprecated

### Accessing the Participant’s Capabilities

var participantRole: CKShare.ParticipantRole

The share’s participant role for the user who retrieves the metadata.

var participantPermission: CKShare.ParticipantPermission

The share’s permissions for the user who retrieves the metadata.

var participantStatus: CKShare.ParticipantAcceptanceStatus

The share’s participation status for the user who retrieves the metadata.

var participantType: CKShare.ParticipantType

The share’s participation type for the user who retrieves the metadata.

Deprecated

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Share Requests

class CKFetchShareMetadataOperation

An operation that fetches metadata for one or more shares.

class CKAcceptSharesOperation

An operation that confirms a user’s participation in a share.

