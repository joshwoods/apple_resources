

- CryptoTokenKit
- TKTokenKeychainContents
-  key(forObjectID:) 

Instance Method

# key(forObjectID:)

Returns the key for a specified object identifier.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func key(forObjectID objectID: TKToken.ObjectID) throws -> TKTokenKeychainKey
```

## Parameters 

`objectID`  

The object identifier for the keychain item.

## Return Value

The key, or `nil` if no key exists.

## See Also

### Accessing Keychain Items

var items: [TKTokenKeychainItem]

Returns all items for token in the keychain.

func certificate(forObjectID: TKToken.ObjectID) throws -> TKTokenKeychainCertificate

Returns the key for a specified object identifier.

