

- CryptoTokenKit
- TKTokenKeychainContents
-  fill(with:) 

Instance Method

# fill(with:)

Fills the keychain with the specified items.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func fill(with items: [TKTokenKeychainItem])
```

## Parameters 

`items`  

The items to be added to the keychain.

## Discussion

All existing items for the token are first removed from the keychain before filling the keychain with `items`.

