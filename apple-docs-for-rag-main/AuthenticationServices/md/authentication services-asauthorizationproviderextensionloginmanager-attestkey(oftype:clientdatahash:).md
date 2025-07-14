

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  attestKey(ofType:clientDataHash:) 

Instance Method

# attestKey(ofType:clientDataHash:)

macOS 15.4+

``` source
func attestKey(
    ofType keyType: ASAuthorizationProviderExtensionKeyType,
    clientDataHash: Data
) async throws -> [SecCertificate]
```

