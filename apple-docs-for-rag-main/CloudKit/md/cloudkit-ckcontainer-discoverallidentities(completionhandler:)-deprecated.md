

- CloudKit
- CKContainer
-  discoverAllIdentities(completionHandler:) Deprecated

Instance Method

# discoverAllIdentities(completionHandler:)

Fetches all user identities that match entries in the user’s Contacts.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.12–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
func discoverAllIdentities(completionHandler: @escaping ([CKUserIdentity]?, (any Error)?) -> Void)
```

``` source
func allUserIdentitiesFromContacts() async throws -> [CKUserIdentity]
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Parameters 

`completionHandler`  

The handler to execute with the fetch results.

## Discussion

The closure doesn’t return a value and takes the following parameters:

- The user identities that match entries in the user’s Contacts.

- An error if a problem occurs, or `nil` if the system successfully completes the request.

This method searches for the users asynchronously and with a low priority. If you want the task to execute with a higher priority, create an instance of CKDiscoverAllUserIdentitiesOperation and configure it to use the necessary priority.

## See Also

### Discovering User Records

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

