

- Apple CryptoKit
- AES
- AES.KeyWrap
-  unwrap(\_:using:) 

Type Method

# unwrap(\_:using:)

Unwraps a key using the AES wrap algorithm.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func unwrap(
    _ wrappedKey: WrappedKey,
    using kek: SymmetricKey
) throws -> SymmetricKey where WrappedKey : DataProtocol
```

## Parameters 

`wrappedKey`  

The key to unwrap.

`kek`  

The key encryption key.

## Return Value

The unwrapped key.

## Discussion

Wrap is an implementation of the AES key wrap algorithm as specified in IETF RFC 3394. The method throws an error is the key was incorrectly wrapped.

