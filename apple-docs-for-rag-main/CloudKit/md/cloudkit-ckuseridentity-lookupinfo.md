

- CloudKit
- CKUserIdentity
-  lookupInfo 

Instance Property

# lookupInfo

The lookup info for retrieving the user identity.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var lookupInfo: CKUserIdentity.LookupInfo? { get }
```

## Discussion

Use this property’s value to retrieve the user identity when using the CKDiscoverUserIdentitiesOperation and CKFetchShareParticipantsOperation operations.

## See Also

### Accessing iCloud Information

var hasiCloudAccount: Bool

A Boolean value that indicates whether the user has an iCloud account.

class LookupInfo

The criteria to use when searching for discoverable iCloud users.

