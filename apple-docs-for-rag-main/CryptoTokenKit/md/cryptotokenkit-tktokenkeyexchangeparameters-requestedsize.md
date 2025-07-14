

- CryptoTokenKit
- TKTokenKeyExchangeParameters
-  requestedSize 

Instance Property

# requestedSize

Returns the requested output size, in bytes, of key exchange result.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var requestedSize: Int { get }
```

## Discussion

This property should be ignored if the output size is not configurable for the specified key exchange algorithm.

## See Also

### Accessing Parameters

var sharedInfo: Data?

Returns shared information typically used during the key derivation (KDF) step of a key exchange algorithm.

