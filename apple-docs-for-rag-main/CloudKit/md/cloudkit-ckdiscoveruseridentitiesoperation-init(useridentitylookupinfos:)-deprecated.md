

- CloudKit
- CKDiscoverUserIdentitiesOperation
-  init(userIdentityLookupInfos:) Deprecated

Initializer

# init(userIdentityLookupInfos:)

Creates an operation for discovering the user identities of the specified lookup infos.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.12–14.0DeprecatedtvOS 10.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
convenience init(userIdentityLookupInfos: [CKUserIdentity.LookupInfo])
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Parameters 

`userIdentityLookupInfos`  

An array that contains instances of CKUserIdentity.LookupInfo. CloudKit uses this parameter as the default value for the userIdentityLookupInfos property. If you specify `nil`, you must assign a value to that property before you execute the operation.

## Discussion

After you create the operation, assign a handler to discoverUserIdentitiesCompletionBlock so that you can process the search results.

## See Also

### Creating an Operation

init()

Creates an operation for discovering user identities.

Deprecated

