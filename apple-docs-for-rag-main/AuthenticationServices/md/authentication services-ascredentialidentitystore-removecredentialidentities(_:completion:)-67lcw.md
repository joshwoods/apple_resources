

- Authentication Services
- ASCredentialIdentityStore
-  removeCredentialIdentities(\_:completion:) 

Instance Method

# removeCredentialIdentities(\_:completion:)

Remove the given credential identities from the store.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func removeCredentialIdentities(
    _ credentialIdentities: [any ASCredentialIdentity],
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func removeCredentialIdentities(_ credentialIdentities: [any ASCredentialIdentity]) async throws
```

## Parameters 

`credentialIdentities`  

A list of credential identities to remove.

`completion`  

An optional completion handler that runs when the operation finishes.

## Discussion

Call this method if the credential store supports incremental updates to remove previously-added credential identities. On failure, this method calls the callback with an error with domain ASCredentialIdentityStoreErrorDomain and doesn’t remove any of the objects in `credentialIdentities` from the store.

## See Also

### Adding and removing credential identities

func saveCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Save the supplied credential identities to the store.

func replaceCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Replaces existing credential identities with new credential identities.

func removeAllCredentialIdentities(((Bool, (any Error)?) -> Void)?)

Removes all existing credential identities from the store.

protocol ASCredentialIdentity

A protocol that credential identity classes conform to that uniquely identifies credentials.

class ASPasskeyCredentialIdentity

A description that uniquely identifies a particular passkey credential.

class ASPasswordCredentialIdentity

A description that uniquely identifies a particular password credential.

