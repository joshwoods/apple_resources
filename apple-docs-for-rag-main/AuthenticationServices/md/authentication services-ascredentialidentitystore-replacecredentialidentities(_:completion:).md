

- Authentication Services
- ASCredentialIdentityStore
-  replaceCredentialIdentities(\_:completion:) 

Instance Method

# replaceCredentialIdentities(\_:completion:)

Replaces existing credential identities with new credential identities.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func replaceCredentialIdentities(
    _ newCredentialIdentities: [any ASCredentialIdentity],
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func replaceCredentialIdentities(_ newCredentialIdentities: [any ASCredentialIdentity]) async throws
```

## Discussion

This method deletes existing credential identities in the store and saves the newly provided credential identity objects. On failure, this method calls the callback with an error with domain ASCredentialIdentityStoreErrorDomain and doesn’t save any of the objects in `newCredentialIdentities` to the store.

## See Also

### Adding and removing credential identities

func saveCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Save the supplied credential identities to the store.

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

