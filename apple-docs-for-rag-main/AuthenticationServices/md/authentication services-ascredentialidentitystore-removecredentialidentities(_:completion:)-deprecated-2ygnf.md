

- Authentication Services
- ASCredentialIdentityStore
-  removeCredentialIdentities(\_:completion:) Deprecated

Instance Method

# removeCredentialIdentities(\_:completion:)

Removes the given credential identities from the store.

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 11.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func removeCredentialIdentities(
    _ credentialIdentities: [ASPasswordCredentialIdentity],
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func removeCredentialIdentities(_ credentialIdentities: [ASPasswordCredentialIdentity]) async throws
```

Deprecated

Use removeCredentialIdentities(_:completion:) instead.

## Parameters 

`credentialIdentities`  

An array of ASPasswordCredentialIdentity objects to remove from the store.

`completion`  

An optional completion handler called after removing the credential identities. If the operation fails, an error with domain ASCredentialIdentityStoreErrorDomain is provided and none of the objects in `credentialIdentities` is removed from the store.

## Discussion

Use this method only if the store supports incremental updates to remove previously added credentials to the store.

## See Also

### Deprecated methods

func saveCredentialIdentities([ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Saves the given credential identities to the store.

Deprecated

func replaceCredentialIdentities(with: [ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Replaces existing credential identities with new credential identities.

Deprecated

