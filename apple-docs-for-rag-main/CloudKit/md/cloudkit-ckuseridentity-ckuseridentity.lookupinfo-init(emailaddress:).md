

- CloudKit
- CKUserIdentity
- CKUserIdentity.LookupInfo
-  init(emailAddress:) 

Initializer

# init(emailAddress:)

Creates a lookup info for the specified email address.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(emailAddress: String)
```

## Parameters 

`emailAddress`  

The email address for looking up the user identity.

## Discussion

After you create a lookup info, use the CKDiscoverUserIdentitiesOperation operation or the CKFetchShareParticipantsOperation operation to retrieve the corresponding user identity.

## See Also

### Creating a Lookup Info

init(phoneNumber: String)

Creates a lookup info for the specified phone number.

init(userRecordID: CKRecord.ID)

Creates a lookup info for the specified user record ID.

