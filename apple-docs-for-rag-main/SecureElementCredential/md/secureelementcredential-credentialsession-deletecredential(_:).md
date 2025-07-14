

- SecureElementCredential
- CredentialSession
-  deleteCredential(\_:) 

Instance Method

# deleteCredential(\_:)

Deletes a credential on the Secure Element.

iOS 18.1+iPadOS 18.1+

``` source
func deleteCredential(_ credential: CredentialSession.Credential) async throws
```

## Parameters 

`credential`  

The credential to delete.

## Mentioned in 

Accessing and using secure element credentials

## See Also

### Managing a credential

func provisionCredential(configurationUUID: UUID, name: String) async throws -> CredentialSession.Credential

Creates a credential in the Secure Element.

