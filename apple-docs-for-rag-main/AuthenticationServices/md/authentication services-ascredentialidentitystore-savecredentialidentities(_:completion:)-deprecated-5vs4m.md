

- Authentication Services
- ASCredentialIdentityStore
-  saveCredentialIdentities(\_:completion:) Deprecated

Instance Method

# saveCredentialIdentities(\_:completion:)

Saves the given credential identities to the store.

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 11.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func saveCredentialIdentities(
    _ credentialIdentities: [ASPasswordCredentialIdentity],
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func saveCredentialIdentities(_ credentialIdentities: [ASPasswordCredentialIdentity]) async throws
```

Deprecated

Use saveCredentialIdentities(_:completion:) instead.

## Parameters 

`credentialIdentities`  

An array of ASPasswordCredentialIdentity objects to save to the store.

`completion`  

An optional completion handler to be called after adding the credential identities. If the operation fails, an error with domain ASCredentialIdentityStoreErrorDomain will be provided and none of the objects in credentialIdentities are saved to the store.

## Discussion

If the store supports incremental updates, call this method to add new credential identities since the last time the store was updated. Otherwise, call this method to pass all credential identities. If some credential identities in `credentialIdentities` already exist in the store, they will be replaced by those from `credentialIdentities`.

## See Also

### Deprecated methods

func replaceCredentialIdentities(with: [ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Replaces existing credential identities with new credential identities.

Deprecated

func removeCredentialIdentities([ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Removes the given credential identities from the store.

Deprecated

