

- Authentication Services
- ASCredentialIdentityStore
-  saveCredentialIdentities(\_:completion:) 

Instance Method

# saveCredentialIdentities(\_:completion:)

Save the supplied credential identities to the store.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func saveCredentialIdentities(
    _ credentialIdentities: [any ASCredentialIdentity],
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func saveCredentialIdentities(_ credentialIdentities: [any ASCredentialIdentity]) async throws
```

## Parameters 

`credentialIdentities`  

A list of credential identities to save.

`completion`  

An optional completion handler that runs when the operation finishes.

## Discussion

Call this method if the credential store supports incremental updates to add new credential identities. Otherwise, call this method passing all credential identities. If any of the credential identities in the `credentialIdentities` array already exist in the store, this method overwrites them with the values in the array.

On failure, this method calls the callback with an error with domain ASCredentialIdentityStoreErrorDomain and doesn’t save any of the objects in `credentialIdentities` to the store.

## See Also

### Adding and removing credential identities

func replaceCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Replaces existing credential identities with new credential identities.

func removeAllCredentialIdentities(((Bool, (any Error)?) -> Void)?)

Removes all existing credential identities from the store.

func removeCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Remove the given credential identities from the store.

protocol ASCredentialIdentity

A protocol that credential identity classes conform to that uniquely identifies credentials.

class ASPasskeyCredentialIdentity

A description that uniquely identifies a particular passkey credential.

class ASPasswordCredentialIdentity

A description that uniquely identifies a particular password credential.

