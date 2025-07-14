

- Authentication Services
- ASCredentialIdentityStore
-  removeAllCredentialIdentities(\_:) 

Instance Method

# removeAllCredentialIdentities(\_:)

Removes all existing credential identities from the store.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func removeAllCredentialIdentities(_ completion: ((Bool, (any Error)?) -> Void)? = nil)
```

``` source
func removeAllCredentialIdentities() async throws
```

## Parameters 

`completion`  

An optional completion handler called after removing all existing credential identities. If the operation fails, an error with domain ASCredentialIdentityStoreErrorDomain is provided and none of the existing credential identities are removed from the store.

## See Also

### Adding and removing credential identities

func saveCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Save the supplied credential identities to the store.

func replaceCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Replaces existing credential identities with new credential identities.

func removeCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Remove the given credential identities from the store.

protocol ASCredentialIdentity

A protocol that credential identity classes conform to that uniquely identifies credentials.

class ASPasskeyCredentialIdentity

A description that uniquely identifies a particular passkey credential.

class ASPasswordCredentialIdentity

A description that uniquely identifies a particular password credential.

