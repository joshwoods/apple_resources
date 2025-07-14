

- Authentication Services
- ASAuthorizationProviderExtensionRegistrationHandler
-  keyWillRotate(for:newKey:loginManager:completion:) 

Instance Method

# keyWillRotate(for:newKey:loginManager:completion:)

macOS 15.0+

``` source
optional func keyWillRotate(
    for keyType: ASAuthorizationProviderExtensionKeyType,
    newKey: SecKey,
    loginManager: ASAuthorizationProviderExtensionLoginManager,
    completion: @escaping (Bool) -> Void
)
```

``` source
optional func keyWillRotate(
    for keyType: ASAuthorizationProviderExtensionKeyType,
    newKey: SecKey,
    loginManager: ASAuthorizationProviderExtensionLoginManager
) async -> Bool
```

