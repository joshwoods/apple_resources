

- Apple CryptoKit
- ChaChaPoly
- ChaChaPoly.Nonce
-  init(data:) 

Initializer

# init(data:)

Creates a nonce from the given data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(data: D) throws where D : DataProtocol
```

## Parameters 

`data`  

A 12-byte data representation of the nonce. The initializer throws an error if the data isn’t 12 bytes long.

## Discussion

Unless your use case calls for a nonce with a specific value, use the init() method to instead create a random nonce.

## See Also

### Creating a nonce

init()

Creates a new random nonce.

