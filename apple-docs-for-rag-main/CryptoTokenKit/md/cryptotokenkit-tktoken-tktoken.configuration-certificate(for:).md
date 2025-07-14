

- CryptoTokenKit
- TKToken
- TKToken.Configuration
-  certificate(for:) 

Instance Method

# certificate(for:)

Returns a certificate from the keychain with the object identifier you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func certificate(for objectID: TKToken.ObjectID) throws -> TKTokenKeychainCertificate
```

## Parameters 

`objectID`  

The identifier for the certificate within the keychain.

## Return Value

The certificate that the keychain stores.

## Discussion

If the certificate the `objectID` specifies isn’t found, the system fills `error` with TKError.Code.objectNotFound.

## See Also

### Retrieving Keys and Certificates

var keychainItems: [TKTokenKeychainItem]

The keychain items associated with this token.

func key(for: TKToken.ObjectID) throws -> TKTokenKeychainKey

Returns a key from the keychain with the object identifier you specify.

