

- CloudKit
- CKUserIdentity
-  hasiCloudAccount 

Instance Property

# hasiCloudAccount

A Boolean value that indicates whether the user has an iCloud account.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var hasiCloudAccount: Bool { get }
```

## Discussion

true if the user identity has an iCloud account; otherwise, false.

## See Also

### Accessing iCloud Information

var lookupInfo: CKUserIdentity.LookupInfo?

The lookup info for retrieving the user identity.

class LookupInfo

The criteria to use when searching for discoverable iCloud users.

