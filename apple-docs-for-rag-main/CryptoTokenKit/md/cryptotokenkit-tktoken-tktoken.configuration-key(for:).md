

- CryptoTokenKit
- TKToken
- TKToken.Configuration
-  key(for:) 

Instance Method

# key(for:)

Returns a key from the keychain with the object identifier you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func key(for objectID: TKToken.ObjectID) throws -> TKTokenKeychainKey
```

## Parameters 

`objectID`  

The identifier for the key within the keychain.

## Return Value

The key that the keychain stores.

## Discussion

If the key the `objectID` specifies isn’t found, the system fills the `error` with TKError.Code.objectNotFound.

## See Also

### Retrieving Keys and Certificates

var keychainItems: [TKTokenKeychainItem]

The keychain items associated with this token.

func certificate(for: TKToken.ObjectID) throws -> TKTokenKeychainCertificate

Returns a certificate from the keychain with the object identifier you specify.

