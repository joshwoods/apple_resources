

- CloudKit
- CKDiscoverUserIdentitiesOperation
-  userIdentityLookupInfos Deprecated

Instance Property

# userIdentityLookupInfos

The lookup info for discovering user identities.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.12–14.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
var userIdentityLookupInfos: [CKUserIdentity.LookupInfo] { get set }
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Discussion

Use this property to view or change the lookup info that CloudKit uses to discover user identities. If you intend to modify this property’s value, do so before you execute the operation or submit it to a queue.

