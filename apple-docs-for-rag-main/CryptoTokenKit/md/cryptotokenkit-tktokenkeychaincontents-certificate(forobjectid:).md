

- CryptoTokenKit
- TKTokenKeychainContents
-  certificate(forObjectID:) 

Instance Method

# certificate(forObjectID:)

Returns the key for a specified object identifier.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func certificate(forObjectID objectID: TKToken.ObjectID) throws -> TKTokenKeychainCertificate
```

## Parameters 

`objectID`  

The object identifier for the keychain item.

## Return Value

The certificate, or `nil` if no certificate exists.

## See Also

### Accessing Keychain Items

var items: [TKTokenKeychainItem]

Returns all items for token in the keychain.

func key(forObjectID: TKToken.ObjectID) throws -> TKTokenKeychainKey

Returns the key for a specified object identifier.

