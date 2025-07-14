

- CloudKit
- CKContainer
-  fetchShareParticipant(withPhoneNumber:completionHandler:) 

Instance Method

# fetchShareParticipant(withPhoneNumber:completionHandler:)

Fetches the share participant with the specified phone number.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func fetchShareParticipant(
    withPhoneNumber phoneNumber: String,
    completionHandler: @escaping (CKShare.Participant?, (any Error)?) -> Void
)
```

``` source
func shareParticipant(forPhoneNumber phoneNumber: String) async throws -> CKShare.Participant
```

## Parameters 

`phoneNumber`  

The share participant’s phone number.

`completionHandler`  

The handler to execute with the fetch results.

## Discussion

The closure doesn’t return a value and takes the following parameters:

- The share participant, or `nil` if CloudKit can’t find the participant.

- An error if a problem occurs, or `nil` if CloudKit successfully retrieves the participant.

This method searches for the share participant asynchronously and with a low priority. If you want the task to execute with a higher priority, create an instance of CKFetchShareParticipantsOperation and configure it to use the necessary priority.

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

func fetchShareParticipant(withUserRecordID: CKRecord.ID, completionHandler: (CKShare.Participant?, (any Error)?) -> Void)

Fetches the share participant with the specified user record ID.

func fetchUserRecordID(completionHandler: (CKRecord.ID?, (any Error)?) -> Void)

Fetches the user record ID of the current user.

let CKCurrentUserDefaultName: String

A constant that provides the current user’s default name.

let CKOwnerDefaultName: String

A constant that provides the default owner’s name.

Deprecated

