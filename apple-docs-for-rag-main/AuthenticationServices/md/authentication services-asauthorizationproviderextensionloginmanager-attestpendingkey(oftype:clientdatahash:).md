

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  attestPendingKey(ofType:clientDataHash:) 

Instance Method

# attestPendingKey(ofType:clientDataHash:)

macOS 15.4+

``` source
func attestPendingKey(
    ofType pendingKeyType: ASAuthorizationProviderExtensionKeyType,
    clientDataHash: Data
) async throws -> [SecCertificate]
```

