

- CloudKit
-  CKCurrentUserDefaultName 

Global Variable

# CKCurrentUserDefaultName

A constant that provides the current user’s default name.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
let CKCurrentUserDefaultName: String
```

## See Also

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

let CKOwnerDefaultName: String

A constant that provides the default owner’s name.

Deprecated

