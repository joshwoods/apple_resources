

- CloudKit
-  CKUserIdentity 

Class

# CKUserIdentity

The identity of a user.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class CKUserIdentity
```

## Overview

A user identity provides identifiable data about an iCloud user, including their name, user record ID, and an email address or phone number. CloudKit retrieves this information from the user’s iCloud account. A user must give their consent to be discoverable before CloudKit can provide this data to your app. For more information, see requestApplicationPermission(_:completionHandler:).

You don’t create instances of this class. Instead, CloudKit provides them in certain contexts. A share’s owner has a user identity, as does each of its participants. When creating participants, CloudKit tries to find iCloud accounts it can use to populate their identities. If CloudKit doesn’t find an account, it sets the identity’s hasiCloudAccount property to false.

You can also discover the identities of your app’s users by executing one of the user discovery operations: CKDiscoverAllUserIdentitiesOperation and CKDiscoverUserIdentitiesOperation. Identities that CloudKit discovers using CKDiscoverAllUserIdentitiesOperation correspond to entries in the device’s Contacts database. These identities contain the identifiers of their Contact records, which you can use to fetch those records from the Contacts database. For more information, see contactIdentifiers.

## Topics

### Accessing iCloud Information

var hasiCloudAccount: Bool

A Boolean value that indicates whether the user has an iCloud account.

var lookupInfo: CKUserIdentity.LookupInfo?

The lookup info for retrieving the user identity.

class LookupInfo

The criteria to use when searching for discoverable iCloud users.

### Accessing User Information

var userRecordID: CKRecord.ID?

The user record ID for the corresponding user record.

var contactIdentifiers: [String]

Identifiers that match contacts in the local Contacts database.

Deprecated

var nameComponents: PersonNameComponents?

The user’s name.

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

### User discovery

class LookupInfo

The criteria to use when searching for discoverable iCloud users.

