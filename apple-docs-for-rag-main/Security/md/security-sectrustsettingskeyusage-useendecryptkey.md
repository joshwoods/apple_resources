

- Security
- SecTrustSettingsKeyUsage
-  useEnDecryptKey 

Type Property

# useEnDecryptKey

The key can be used to encrypt or decrypt (wrap or unwrap) a key.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var useEnDecryptKey: SecTrustSettingsKeyUsage { get }
```

## Discussion

Private keys must be wrapped before they can be exported from a keychain.

