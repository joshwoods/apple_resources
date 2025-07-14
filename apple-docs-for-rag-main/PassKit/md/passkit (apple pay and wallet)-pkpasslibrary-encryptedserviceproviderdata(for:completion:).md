

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  encryptedServiceProviderData(for:completion:) 

Instance Method

# encryptedServiceProviderData(for:completion:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.12+visionOS 1.0+watchOS 9.0+

``` source
func encryptedServiceProviderData(
    for secureElementPass: PKSecureElementPass,
    completion: @escaping ([AnyHashable : Any]?, (any Error)?) -> Void
)
```

``` source
func encryptedServiceProviderData(for secureElementPass: PKSecureElementPass) async throws -> [AnyHashable : Any]
```

