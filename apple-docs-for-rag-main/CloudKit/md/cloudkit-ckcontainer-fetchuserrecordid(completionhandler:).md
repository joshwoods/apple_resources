

- CloudKit
- CKContainer
-  fetchUserRecordID(completionHandler:) 

Instance Method

# fetchUserRecordID(completionHandler:)

Fetches the user record ID of the current user.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func fetchUserRecordID(completionHandler: @escaping (CKRecord.ID?, (any Error)?) -> Void)
```

``` source
func userRecordID() async throws -> CKRecord.ID
```

## Parameters 

`completionHandler`  

The handler to execute with the fetch results.

## Discussion

The closure doesn’t return a value and takes the following parameters:

- The user record ID, or `nil` if the user disables iCloud Drive or the device doesn’t have an iCloud account.

- An error if a problem occurs, or `nil` if CloudKit successfully retrieves the user record ID.

CloudKit returns a CKError.Code.notAuthenticated error when any of the following conditions are met:

- The device has an iCloud account but the user disables iCloud Drive.

- The device has an iCloud account with restricted access.

- The device doesn’t have an iCloud account.

Note

At startup, fetching the user record ID may take longer while CloudKit makes the initial iCloud account request. After the initial fetch, accessing the ID generally takes less time.

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

let CKCurrentUserDefaultName: String

A constant that provides the current user’s default name.

let CKOwnerDefaultName: String

A constant that provides the default owner’s name.

Deprecated

