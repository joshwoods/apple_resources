

- CloudKit
- CKDiscoverUserIdentitiesOperation
-  init() Deprecated

Initializer

# init()

Creates an operation for discovering user identities.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.12–14.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
init()
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Discussion

You can use the operation only once. Create a new operation for each subsequent search.

## See Also

### Creating an Operation

convenience init(userIdentityLookupInfos: [CKUserIdentity.LookupInfo])

Creates an operation for discovering the user identities of the specified lookup infos.

Deprecated

