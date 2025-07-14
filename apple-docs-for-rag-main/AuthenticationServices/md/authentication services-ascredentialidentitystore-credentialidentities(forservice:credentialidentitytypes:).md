

- Authentication Services
- ASCredentialIdentityStore
-  credentialIdentities(forService:credentialIdentityTypes:) 

Instance Method

# credentialIdentities(forService:credentialIdentityTypes:)

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+visionOS 1.1+

``` source
func credentialIdentities(
    forService serviceIdentifier: ASCredentialServiceIdentifier? = nil,
    credentialIdentityTypes: ASCredentialIdentityStore.IdentityTypes = []
) async -> [any ASCredentialIdentity]
```

