

- Authentication Services
- ASCredentialIdentityStore
-  replaceCredentialIdentities(with:completion:) Deprecated

Instance Method

# replaceCredentialIdentities(with:completion:)

Replaces existing credential identities with new credential identities.

iOS 12.0–17.0DeprecatediPadOS 12.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 11.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func replaceCredentialIdentities(
    with newCredentialIdentities: [ASPasswordCredentialIdentity],
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func replaceCredentialIdentities(with newCredentialIdentities: [ASPasswordCredentialIdentity]) async throws
```

Deprecated

Use replaceCredentialIdentities(_:completion:) instead.

## Parameters 

`newCredentialIdentities`  

An array of new credential identity objects to replace the old ones.

`completion`  

An optional completion block called after the operation finishes.

## Discussion

This method deletes existing credential identities that are persisted in the store and saves the newly provided credential identity objects. If the operation fails, an error with domain ASCredentialIdentityStoreErrorDomain is provided and none of the new credential identities are saved.

## See Also

### Deprecated methods

func saveCredentialIdentities([ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Saves the given credential identities to the store.

Deprecated

func removeCredentialIdentities([ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Removes the given credential identities from the store.

Deprecated

