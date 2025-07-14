

- CryptoTokenKit
- TKTokenKeyExchangeParameters
-  sharedInfo 

Instance Property

# sharedInfo

Returns shared information typically used during the key derivation (KDF) step of a key exchange algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var sharedInfo: Data? { get }
```

## Discussion

This property should be ignored if shared information isn’t used by the specified key exchange algorithm.

## See Also

### Accessing Parameters

var requestedSize: Int

Returns the requested output size, in bytes, of key exchange result.

