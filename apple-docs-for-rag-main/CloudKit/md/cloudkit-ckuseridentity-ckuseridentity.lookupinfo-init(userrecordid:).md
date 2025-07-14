

- CloudKit
- CKUserIdentity
- CKUserIdentity.LookupInfo
-  init(userRecordID:) 

Initializer

# init(userRecordID:)

Creates a lookup info for the specified user record ID.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(userRecordID: CKRecord.ID)
```

## Parameters 

`userRecordID`  

The user record ID for looking up the user identity.

## Discussion

After you create a lookup info, use the CKDiscoverUserIdentitiesOperation operation or the CKFetchShareParticipantsOperation operation to retrieve the corresponding user identity.

## See Also

### Creating a Lookup Info

init(emailAddress: String)

Creates a lookup info for the specified email address.

init(phoneNumber: String)

Creates a lookup info for the specified phone number.

