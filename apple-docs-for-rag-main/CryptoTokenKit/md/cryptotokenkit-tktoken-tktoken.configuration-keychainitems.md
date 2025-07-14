

- CryptoTokenKit
- TKToken
- TKToken.Configuration
-  keychainItems 

Instance Property

# keychainItems

The keychain items associated with this token.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var keychainItems: [TKTokenKeychainItem] { get set }
```

## See Also

### Retrieving Keys and Certificates

func certificate(for: TKToken.ObjectID) throws -> TKTokenKeychainCertificate

Returns a certificate from the keychain with the object identifier you specify.

func key(for: TKToken.ObjectID) throws -> TKTokenKeychainKey

Returns a key from the keychain with the object identifier you specify.

