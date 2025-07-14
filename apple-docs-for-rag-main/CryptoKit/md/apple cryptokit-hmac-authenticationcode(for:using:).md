

- Apple CryptoKit
- HMAC
-  authenticationCode(for:using:) 

Type Method

# authenticationCode(for:using:)

Computes a message authentication code for the given data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func authenticationCode(
    for data: D,
    using key: SymmetricKey
) -> HMAC.MAC where D : DataProtocol
```

## Parameters 

`data`  

The data for which to compute the authentication code.

`key`  

The symmetric key used to secure the computation.

## Return Value

The message authentication code.

