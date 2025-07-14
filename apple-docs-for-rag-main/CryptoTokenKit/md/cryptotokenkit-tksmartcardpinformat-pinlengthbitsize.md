

- CryptoTokenKit
- TKSmartCardPINFormat
-  pinLengthBitSize 

Instance Property

# pinLengthBitSize

The size, in bits, of the PIN length field. If set to `0`, PIN length is not written. `0` by default.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
var pinLengthBitSize: Int { get set }
```

## See Also

### Configuring PIN Formatting

var charset: TKSmartCardPINFormat.Charset

The format of PIN characters. `TKSmartCardPINCharsetNumeric` by default.

var encoding: TKSmartCardPINFormat.Encoding

The encoding of PIN characters. `TKSmartCardPINEncodingASCII` by default.

var minPINLength: Int

The minimum number of characters to form a valid PIN. `4` by default.

var maxPINLength: Int

The maximum number of characters to form a valid PIN. `8` by default.

var pinBlockByteLength: Int

The total length of the PIN block in bytes. `8` by default.

var pinJustification: TKSmartCardPINFormat.Justification

The justification within the PIN block. `TKSmartCardPINJustificationLeft` by default.

var pinBitOffset: Int

The offset, in bits, within the PIN block to mark a location for filling in the formatted PIN, which is justified with respect to the pinJustification property value. `0` by default.

var pinLengthBitOffset: Int

The offset, in bits, within the PIN block to mark a location for filling in the PIN length, which is always left justified. `0` by default.

