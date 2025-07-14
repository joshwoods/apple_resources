

- CloudKit
- CKContainer
-  discoverUserIdentity(withEmailAddress:completionHandler:) Deprecated

Instance Method

# discoverUserIdentity(withEmailAddress:completionHandler:)

Fetches the user identity for the specified email address.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.12–14.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
func discoverUserIdentity(
    withEmailAddress email: String,
    completionHandler: @escaping (CKUserIdentity?, (any Error)?) -> Void
)
```

``` source
func userIdentity(forEmailAddress email: String) async throws -> CKUserIdentity?
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Parameters 

`email`  

The user’s email address.

`completionHandler`  

The handler to execute with the fetch results.

## Discussion

This closure doesn’t return a value and takes the following parameters:

- The user identity for the email address, or `nil` if CloudKit can’t find an identity.

- An error if a problem occurs, or `nil` if CloudKit successfully fetches a user identity.

Use this method to retrieve the identity of a user who the current user knows. The user you’re searching for must meet the following criteria:

- The user must be in the current user’s Contacts.

- The user has run the app.

- The user grants the userDiscoverability permission for the container.

This method searches for the user asynchronously and with a low priority. If you want the task to execute the request with a higher priority, create an instance of CKDiscoverUserIdentitiesOperation and configure it to use the necessary priority.

## See Also

### Discovering User Records

func discoverAllIdentities(completionHandler: ([CKUserIdentity]?, (any Error)?) -> Void)

Fetches all user identities that match entries in the user’s Contacts.

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

