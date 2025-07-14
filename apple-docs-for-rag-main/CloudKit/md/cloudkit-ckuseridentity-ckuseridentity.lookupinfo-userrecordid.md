

- CloudKit
- CKUserIdentity
- CKUserIdentity.LookupInfo
-  userRecordID 

Instance Property

# userRecordID

The ID of the user record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var userRecordID: CKRecord.ID? { get }
```

## Discussion

Use this value to retrieve the user record for the user identity. The user record doesn’t contain any personal information about the user, by default. You can add data to the user record, but you shouldn’t add anything sensitive.

## See Also

### Accessing the Criteria

var emailAddress: String?

The user’s email address.

var phoneNumber: String?

The user’s phone number.

