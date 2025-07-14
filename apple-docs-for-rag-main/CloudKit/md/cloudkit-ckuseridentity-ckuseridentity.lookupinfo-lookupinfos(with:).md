

- CloudKit
- CKUserIdentity
- CKUserIdentity.LookupInfo
-  lookupInfos(with:) 

Type Method

# lookupInfos(with:)

Returns an array of lookup infos for the specifed user record IDs.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func lookupInfos(with recordIDs: [CKRecord.ID]) -> [CKUserIdentity.LookupInfo]
```

## Parameters 

`recordIDs`  

The user record IDs for looking up the user identities.

## Discussion

Use the values that this method returns in an CKDiscoverUserIdentitiesOperation operation or an CKFetchShareParticipantsOperation operation to retrieve the corresponding user identities.

## See Also

### Creating Multiple Lookup Infos

class func lookupInfos(withEmails: [String]) -> [CKUserIdentity.LookupInfo]

Returns an array of lookup infos for the specifed email addresses.

class func lookupInfos(withPhoneNumbers: [String]) -> [CKUserIdentity.LookupInfo]

Returns an array of lookup infos for the specifed phone numbers.

