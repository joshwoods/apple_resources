

- CloudKit
- CKUserIdentity
-  CKUserIdentity.LookupInfo 

Class

# CKUserIdentity.LookupInfo

The criteria to use when searching for discoverable iCloud users.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class LookupInfo
```

## Overview

Use this object when you want to discover the identities of your app’s users with CKDiscoverUserIdentitiesOperation, or to create a share’s participants with CKFetchShareParticipantsOperation.

You create individual instances by providing an email address, phone number, or user record ID. Alternatively, create an array of objects all at once by using one of the convenience methods, such as lookupInfos(withEmails:).

## Topics

### Creating a Lookup Info

init(emailAddress: String)

Creates a lookup info for the specified email address.

init(phoneNumber: String)

Creates a lookup info for the specified phone number.

init(userRecordID: CKRecord.ID)

Creates a lookup info for the specified user record ID.

### Creating Multiple Lookup Infos

class func lookupInfos(withEmails: [String]) -> [CKUserIdentity.LookupInfo]

Returns an array of lookup infos for the specifed email addresses.

class func lookupInfos(withPhoneNumbers: [String]) -> [CKUserIdentity.LookupInfo]

Returns an array of lookup infos for the specifed phone numbers.

class func lookupInfos(with: [CKRecord.ID]) -> [CKUserIdentity.LookupInfo]

Returns an array of lookup infos for the specifed user record IDs.

### Accessing the Criteria

var emailAddress: String?

The user’s email address.

var phoneNumber: String?

The user’s phone number.

var userRecordID: CKRecord.ID?

The ID of the user record.

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

class CKUserIdentity

The identity of a user.

