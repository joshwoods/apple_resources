

- Apple CryptoKit
- HPKE
- HPKE.AEAD
-  HPKE.AEAD.exportOnly 

Case

# HPKE.AEAD.exportOnly

An export-only mode.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case exportOnly
```

## Discussion

In export-only mode, HPKE negotiates key derivation, but you can’t use it to encrypt or decrypt data.

